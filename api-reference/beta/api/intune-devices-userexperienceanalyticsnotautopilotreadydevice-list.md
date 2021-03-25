---
title: Список userExperienceAnalyticsNotAutopilotReadyDevices
description: Список свойств и связей объектов userExperienceAnalyticsNotAutopilotReadyDevice.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 75f747552f3ff080385862b3540cca36fc88ae4b
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51159495"
---
# <a name="list-userexperienceanalyticsnotautopilotreadydevices"></a><span data-ttu-id="e5128-103">Список userExperienceAnalyticsNotAutopilotReadyDevices</span><span class="sxs-lookup"><span data-stu-id="e5128-103">List userExperienceAnalyticsNotAutopilotReadyDevices</span></span>

<span data-ttu-id="e5128-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5128-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e5128-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5128-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e5128-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e5128-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5128-107">Список свойств и связей [объектов userExperienceAnalyticsNotAutopilotReadyDevice.](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md)</span><span class="sxs-lookup"><span data-stu-id="e5128-107">List properties and relationships of the [userExperienceAnalyticsNotAutopilotReadyDevice](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e5128-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e5128-108">Prerequisites</span></span>
<span data-ttu-id="e5128-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5128-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5128-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e5128-111">Permission type</span></span>|<span data-ttu-id="e5128-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e5128-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e5128-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e5128-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e5128-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5128-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e5128-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e5128-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e5128-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5128-116">Not supported.</span></span>|
|<span data-ttu-id="e5128-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="e5128-117">Application</span></span>|<span data-ttu-id="e5128-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5128-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e5128-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e5128-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsNotAutopilotReadyDevice
```

## <a name="request-headers"></a><span data-ttu-id="e5128-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e5128-120">Request headers</span></span>
|<span data-ttu-id="e5128-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e5128-121">Header</span></span>|<span data-ttu-id="e5128-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e5128-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e5128-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5128-123">Authorization</span></span>|<span data-ttu-id="e5128-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e5128-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e5128-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e5128-125">Accept</span></span>|<span data-ttu-id="e5128-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e5128-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5128-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e5128-127">Request body</span></span>
<span data-ttu-id="e5128-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e5128-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e5128-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5128-129">Response</span></span>
<span data-ttu-id="e5128-130">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [userExperienceAnalyticsNotAutopilotReadyDevice](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e5128-130">If successful, this method returns a `200 OK` response code and a collection of [userExperienceAnalyticsNotAutopilotReadyDevice](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5128-131">Пример</span><span class="sxs-lookup"><span data-stu-id="e5128-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e5128-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e5128-132">Request</span></span>
<span data-ttu-id="e5128-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e5128-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsNotAutopilotReadyDevice
```

### <a name="response"></a><span data-ttu-id="e5128-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5128-134">Response</span></span>
<span data-ttu-id="e5128-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e5128-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 548

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsNotAutopilotReadyDevice",
      "id": "11c3ffd7-ffd7-11c3-d7ff-c311d7ffc311",
      "deviceName": "Device Name value",
      "serialNumber": "Serial Number value",
      "manufacturer": "Manufacturer value",
      "model": "Model value",
      "managedBy": "Managed By value",
      "autoPilotRegistered": true,
      "autoPilotProfileAssigned": true,
      "azureAdRegistered": "yes",
      "azureAdJoinType": "Azure Ad Join Type value"
    }
  ]
}
```




