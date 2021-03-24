---
title: Список deviceManagementIntentDeviceStates
description: Список свойств и связей объектов deviceManagementIntentDeviceState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cd6b1b1e0226e7643d34ca63bd54d9da45e898b0
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51128742"
---
# <a name="list-devicemanagementintentdevicestates"></a><span data-ttu-id="77f05-103">Список deviceManagementIntentDeviceStates</span><span class="sxs-lookup"><span data-stu-id="77f05-103">List deviceManagementIntentDeviceStates</span></span>

<span data-ttu-id="77f05-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77f05-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="77f05-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77f05-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="77f05-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="77f05-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77f05-107">Список свойств и связей [объектов deviceManagementIntentDeviceState.](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)</span><span class="sxs-lookup"><span data-stu-id="77f05-107">List properties and relationships of the [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="77f05-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="77f05-108">Prerequisites</span></span>
<span data-ttu-id="77f05-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77f05-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77f05-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="77f05-111">Permission type</span></span>|<span data-ttu-id="77f05-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="77f05-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77f05-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="77f05-113">Delegated (work or school account)</span></span>|<span data-ttu-id="77f05-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77f05-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="77f05-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="77f05-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77f05-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77f05-116">Not supported.</span></span>|
|<span data-ttu-id="77f05-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="77f05-117">Application</span></span>|<span data-ttu-id="77f05-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77f05-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="77f05-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="77f05-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents/{deviceManagementIntentId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="77f05-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="77f05-120">Request headers</span></span>
|<span data-ttu-id="77f05-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="77f05-121">Header</span></span>|<span data-ttu-id="77f05-122">Значение</span><span class="sxs-lookup"><span data-stu-id="77f05-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77f05-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="77f05-123">Authorization</span></span>|<span data-ttu-id="77f05-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="77f05-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77f05-125">Accept</span><span class="sxs-lookup"><span data-stu-id="77f05-125">Accept</span></span>|<span data-ttu-id="77f05-126">application/json</span><span class="sxs-lookup"><span data-stu-id="77f05-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77f05-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="77f05-127">Request body</span></span>
<span data-ttu-id="77f05-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="77f05-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="77f05-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="77f05-129">Response</span></span>
<span data-ttu-id="77f05-130">В случае успешного выполнения этот метод возвращает код ответа и коллекцию объектов `200 OK` [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="77f05-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77f05-131">Пример</span><span class="sxs-lookup"><span data-stu-id="77f05-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="77f05-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="77f05-132">Request</span></span>
<span data-ttu-id="77f05-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="77f05-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/deviceStates
```

### <a name="response"></a><span data-ttu-id="77f05-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="77f05-134">Response</span></span>
<span data-ttu-id="77f05-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="77f05-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




