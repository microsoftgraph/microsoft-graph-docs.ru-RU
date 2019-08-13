---
title: Список Девицеманажементинтентдевицестатес
description: Список свойств и связей объектов Девицеманажементинтентдевицестате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 007c67cd0c51d75b425b703b9fc2e575c2013663
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36343610"
---
# <a name="list-devicemanagementintentdevicestates"></a><span data-ttu-id="01679-103">Список Девицеманажементинтентдевицестатес</span><span class="sxs-lookup"><span data-stu-id="01679-103">List deviceManagementIntentDeviceStates</span></span>

> <span data-ttu-id="01679-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01679-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="01679-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="01679-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="01679-106">Список свойств и связей объектов [девицеманажементинтентдевицестате](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="01679-106">List properties and relationships of the [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="01679-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="01679-107">Prerequisites</span></span>
<span data-ttu-id="01679-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01679-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01679-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="01679-110">Permission type</span></span>|<span data-ttu-id="01679-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="01679-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="01679-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="01679-112">Delegated (work or school account)</span></span>|<span data-ttu-id="01679-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="01679-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="01679-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="01679-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="01679-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01679-115">Not supported.</span></span>|
|<span data-ttu-id="01679-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="01679-116">Application</span></span>|<span data-ttu-id="01679-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="01679-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="01679-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="01679-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents/{deviceManagementIntentId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="01679-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="01679-119">Request headers</span></span>
|<span data-ttu-id="01679-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="01679-120">Header</span></span>|<span data-ttu-id="01679-121">Значение</span><span class="sxs-lookup"><span data-stu-id="01679-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="01679-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="01679-122">Authorization</span></span>|<span data-ttu-id="01679-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="01679-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="01679-124">Accept</span><span class="sxs-lookup"><span data-stu-id="01679-124">Accept</span></span>|<span data-ttu-id="01679-125">application/json</span><span class="sxs-lookup"><span data-stu-id="01679-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="01679-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="01679-126">Request body</span></span>
<span data-ttu-id="01679-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="01679-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="01679-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="01679-128">Response</span></span>
<span data-ttu-id="01679-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [девицеманажементинтентдевицестате](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="01679-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01679-130">Пример</span><span class="sxs-lookup"><span data-stu-id="01679-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="01679-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="01679-131">Request</span></span>
<span data-ttu-id="01679-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="01679-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/deviceStates
```

### <a name="response"></a><span data-ttu-id="01679-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="01679-133">Response</span></span>
<span data-ttu-id="01679-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="01679-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






