---
title: Список Девицеманажементинтентдевицестатес
description: Список свойств и связей объектов Девицеманажементинтентдевицестате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 74ae9224686383243c31431305bab8694fa27b2a
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33915918"
---
# <a name="list-devicemanagementintentdevicestates"></a><span data-ttu-id="3ac01-103">Список Девицеманажементинтентдевицестатес</span><span class="sxs-lookup"><span data-stu-id="3ac01-103">List deviceManagementIntentDeviceStates</span></span>

> <span data-ttu-id="3ac01-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ac01-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3ac01-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3ac01-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ac01-106">Список свойств и связей объектов [девицеманажементинтентдевицестате](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="3ac01-106">List properties and relationships of the [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3ac01-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3ac01-107">Prerequisites</span></span>
<span data-ttu-id="3ac01-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ac01-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ac01-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3ac01-110">Permission type</span></span>|<span data-ttu-id="3ac01-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3ac01-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3ac01-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3ac01-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3ac01-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ac01-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="3ac01-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3ac01-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3ac01-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ac01-115">Not supported.</span></span>|
|<span data-ttu-id="3ac01-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3ac01-116">Application</span></span>|<span data-ttu-id="3ac01-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ac01-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3ac01-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3ac01-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents/{deviceManagementIntentId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="3ac01-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3ac01-119">Request headers</span></span>
|<span data-ttu-id="3ac01-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3ac01-120">Header</span></span>|<span data-ttu-id="3ac01-121">Значение</span><span class="sxs-lookup"><span data-stu-id="3ac01-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3ac01-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3ac01-122">Authorization</span></span>|<span data-ttu-id="3ac01-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3ac01-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3ac01-124">Accept</span><span class="sxs-lookup"><span data-stu-id="3ac01-124">Accept</span></span>|<span data-ttu-id="3ac01-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3ac01-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3ac01-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3ac01-126">Request body</span></span>
<span data-ttu-id="3ac01-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3ac01-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3ac01-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="3ac01-128">Response</span></span>
<span data-ttu-id="3ac01-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [девицеманажементинтентдевицестате](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3ac01-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ac01-130">Пример</span><span class="sxs-lookup"><span data-stu-id="3ac01-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="3ac01-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="3ac01-131">Request</span></span>
<span data-ttu-id="3ac01-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3ac01-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/deviceStates
```

### <a name="response"></a><span data-ttu-id="3ac01-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ac01-133">Response</span></span>
<span data-ttu-id="3ac01-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3ac01-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




