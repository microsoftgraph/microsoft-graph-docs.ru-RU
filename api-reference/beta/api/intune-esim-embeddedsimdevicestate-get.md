---
title: Получение Ембеддедсимдевицестате
description: Чтение свойств и связей объекта Ембеддедсимдевицестате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 29628015284d344dcb7c759e1cadde7faf41e5a7
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36355733"
---
# <a name="get-embeddedsimdevicestate"></a><span data-ttu-id="39dd4-103">Получение Ембеддедсимдевицестате</span><span class="sxs-lookup"><span data-stu-id="39dd4-103">Get embeddedSIMDeviceState</span></span>

> <span data-ttu-id="39dd4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39dd4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="39dd4-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="39dd4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="39dd4-106">Чтение свойств и связей объекта [ембеддедсимдевицестате](../resources/intune-esim-embeddedsimdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="39dd4-106">Read properties and relationships of the [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="39dd4-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="39dd4-107">Prerequisites</span></span>
<span data-ttu-id="39dd4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39dd4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39dd4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="39dd4-110">Permission type</span></span>|<span data-ttu-id="39dd4-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="39dd4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="39dd4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="39dd4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="39dd4-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="39dd4-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="39dd4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="39dd4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="39dd4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39dd4-115">Not supported.</span></span>|
|<span data-ttu-id="39dd4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="39dd4-116">Application</span></span>|<span data-ttu-id="39dd4-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="39dd4-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="39dd4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="39dd4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates/{embeddedSIMDeviceStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="39dd4-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="39dd4-119">Optional query parameters</span></span>
<span data-ttu-id="39dd4-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="39dd4-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="39dd4-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="39dd4-121">Request headers</span></span>
|<span data-ttu-id="39dd4-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="39dd4-122">Header</span></span>|<span data-ttu-id="39dd4-123">Значение</span><span class="sxs-lookup"><span data-stu-id="39dd4-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="39dd4-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="39dd4-124">Authorization</span></span>|<span data-ttu-id="39dd4-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="39dd4-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="39dd4-126">Accept</span><span class="sxs-lookup"><span data-stu-id="39dd4-126">Accept</span></span>|<span data-ttu-id="39dd4-127">application/json</span><span class="sxs-lookup"><span data-stu-id="39dd4-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="39dd4-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="39dd4-128">Request body</span></span>
<span data-ttu-id="39dd4-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="39dd4-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="39dd4-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="39dd4-130">Response</span></span>
<span data-ttu-id="39dd4-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [ембеддедсимдевицестате](../resources/intune-esim-embeddedsimdevicestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="39dd4-131">If successful, this method returns a `200 OK` response code and [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="39dd4-132">Пример</span><span class="sxs-lookup"><span data-stu-id="39dd4-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="39dd4-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="39dd4-133">Request</span></span>
<span data-ttu-id="39dd4-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="39dd4-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates/{embeddedSIMDeviceStateId}
```

### <a name="response"></a><span data-ttu-id="39dd4-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="39dd4-135">Response</span></span>
<span data-ttu-id="39dd4-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="39dd4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 568

{
  "value": {
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
}
```






