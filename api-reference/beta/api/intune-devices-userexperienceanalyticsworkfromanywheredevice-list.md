---
title: Список userExperienceAnalyticsWorkFromAnywhereDevices
description: Список свойств и связей объектов userExperienceAnalyticsWorkFromAnywhereDevice.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 33b0659d3ca6c86b3c57c10fb17625bcdb91bf09
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51869007"
---
# <a name="list-userexperienceanalyticsworkfromanywheredevices"></a><span data-ttu-id="0d453-103">Список userExperienceAnalyticsWorkFromAnywhereDevices</span><span class="sxs-lookup"><span data-stu-id="0d453-103">List userExperienceAnalyticsWorkFromAnywhereDevices</span></span>

<span data-ttu-id="0d453-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d453-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0d453-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d453-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0d453-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0d453-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d453-107">Список свойств и связей [объектов userExperienceAnalyticsWorkFromAnywhereDevice.](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md)</span><span class="sxs-lookup"><span data-stu-id="0d453-107">List properties and relationships of the [userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0d453-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0d453-108">Prerequisites</span></span>
<span data-ttu-id="0d453-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d453-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d453-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0d453-111">Permission type</span></span>|<span data-ttu-id="0d453-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0d453-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0d453-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0d453-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0d453-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d453-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="0d453-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0d453-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0d453-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d453-116">Not supported.</span></span>|
|<span data-ttu-id="0d453-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="0d453-117">Application</span></span>|<span data-ttu-id="0d453-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d453-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0d453-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0d453-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsWorkFromAnywhereMetrics/{userExperienceAnalyticsWorkFromAnywhereMetricId}/metricDevices
```

## <a name="request-headers"></a><span data-ttu-id="0d453-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0d453-120">Request headers</span></span>
|<span data-ttu-id="0d453-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0d453-121">Header</span></span>|<span data-ttu-id="0d453-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0d453-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0d453-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0d453-123">Authorization</span></span>|<span data-ttu-id="0d453-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0d453-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0d453-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0d453-125">Accept</span></span>|<span data-ttu-id="0d453-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0d453-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d453-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0d453-127">Request body</span></span>
<span data-ttu-id="0d453-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0d453-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0d453-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d453-129">Response</span></span>
<span data-ttu-id="0d453-130">В случае успеха этот метод возвращает код ответа и коллекцию объектов `200 OK` [userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="0d453-130">If successful, this method returns a `200 OK` response code and a collection of [userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d453-131">Пример</span><span class="sxs-lookup"><span data-stu-id="0d453-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="0d453-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="0d453-132">Request</span></span>
<span data-ttu-id="0d453-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0d453-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsWorkFromAnywhereMetrics/{userExperienceAnalyticsWorkFromAnywhereMetricId}/metricDevices
```

### <a name="response"></a><span data-ttu-id="0d453-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d453-134">Response</span></span>
<span data-ttu-id="0d453-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0d453-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 639

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsWorkFromAnywhereDevice",
      "id": "83d5adfc-adfc-83d5-fcad-d583fcadd583",
      "deviceName": "Device Name value",
      "serialNumber": "Serial Number value",
      "manufacturer": "Manufacturer value",
      "model": "Model value",
      "ownership": "Ownership value",
      "managedBy": "Managed By value",
      "autoPilotRegistered": true,
      "autoPilotProfileAssigned": true,
      "azureAdRegistered": true,
      "azureAdDeviceId": "Azure Ad Device Id value",
      "azureAdJoinType": "Azure Ad Join Type value"
    }
  ]
}
```




