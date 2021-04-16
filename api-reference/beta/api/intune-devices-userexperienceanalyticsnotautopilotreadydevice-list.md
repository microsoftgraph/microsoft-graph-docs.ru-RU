---
title: Список userExperienceAnalyticsNotAutopilotReadyDevices
description: Список свойств и связей объектов userExperienceAnalyticsNotAutopilotReadyDevice.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: aa0fffb7a5589d618c566b3845968a4f4ca6ae3f
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867576"
---
# <a name="list-userexperienceanalyticsnotautopilotreadydevices"></a><span data-ttu-id="4f6dc-103">Список userExperienceAnalyticsNotAutopilotReadyDevices</span><span class="sxs-lookup"><span data-stu-id="4f6dc-103">List userExperienceAnalyticsNotAutopilotReadyDevices</span></span>

<span data-ttu-id="4f6dc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f6dc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4f6dc-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f6dc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4f6dc-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4f6dc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f6dc-107">Список свойств и связей [объектов userExperienceAnalyticsNotAutopilotReadyDevice.](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md)</span><span class="sxs-lookup"><span data-stu-id="4f6dc-107">List properties and relationships of the [userExperienceAnalyticsNotAutopilotReadyDevice](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4f6dc-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4f6dc-108">Prerequisites</span></span>
<span data-ttu-id="4f6dc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f6dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f6dc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4f6dc-111">Permission type</span></span>|<span data-ttu-id="4f6dc-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4f6dc-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f6dc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4f6dc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4f6dc-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f6dc-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="4f6dc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4f6dc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f6dc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f6dc-116">Not supported.</span></span>|
|<span data-ttu-id="4f6dc-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="4f6dc-117">Application</span></span>|<span data-ttu-id="4f6dc-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f6dc-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f6dc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4f6dc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsNotAutopilotReadyDevice
```

## <a name="request-headers"></a><span data-ttu-id="4f6dc-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4f6dc-120">Request headers</span></span>
|<span data-ttu-id="4f6dc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4f6dc-121">Header</span></span>|<span data-ttu-id="4f6dc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4f6dc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4f6dc-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4f6dc-123">Authorization</span></span>|<span data-ttu-id="4f6dc-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4f6dc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4f6dc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4f6dc-125">Accept</span></span>|<span data-ttu-id="4f6dc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4f6dc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f6dc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4f6dc-127">Request body</span></span>
<span data-ttu-id="4f6dc-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4f6dc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4f6dc-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f6dc-129">Response</span></span>
<span data-ttu-id="4f6dc-130">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [userExperienceAnalyticsNotAutopilotReadyDevice](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="4f6dc-130">If successful, this method returns a `200 OK` response code and a collection of [userExperienceAnalyticsNotAutopilotReadyDevice](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f6dc-131">Пример</span><span class="sxs-lookup"><span data-stu-id="4f6dc-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="4f6dc-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f6dc-132">Request</span></span>
<span data-ttu-id="4f6dc-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4f6dc-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsNotAutopilotReadyDevice
```

### <a name="response"></a><span data-ttu-id="4f6dc-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f6dc-134">Response</span></span>
<span data-ttu-id="4f6dc-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4f6dc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 547

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
      "azureAdRegistered": true,
      "azureAdJoinType": "Azure Ad Join Type value"
    }
  ]
}
```




