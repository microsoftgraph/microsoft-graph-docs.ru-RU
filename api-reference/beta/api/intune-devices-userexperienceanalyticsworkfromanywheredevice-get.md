---
title: Get userExperienceAnalyticsWorkFromAnywhereDevice
description: Чтение свойств и связей объекта userExperienceAnalyticsWorkFromAnywhereDevice.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 49efeea6ec112fe569daa36a8121d3d32ea03694
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51869016"
---
# <a name="get-userexperienceanalyticsworkfromanywheredevice"></a><span data-ttu-id="1ffb8-103">Get userExperienceAnalyticsWorkFromAnywhereDevice</span><span class="sxs-lookup"><span data-stu-id="1ffb8-103">Get userExperienceAnalyticsWorkFromAnywhereDevice</span></span>

<span data-ttu-id="1ffb8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ffb8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1ffb8-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ffb8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1ffb8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1ffb8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ffb8-107">Чтение свойств и связей [объекта userExperienceAnalyticsWorkFromAnywhereDevice.](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md)</span><span class="sxs-lookup"><span data-stu-id="1ffb8-107">Read properties and relationships of the [userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1ffb8-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1ffb8-108">Prerequisites</span></span>
<span data-ttu-id="1ffb8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ffb8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ffb8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1ffb8-111">Permission type</span></span>|<span data-ttu-id="1ffb8-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1ffb8-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1ffb8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1ffb8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1ffb8-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ffb8-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="1ffb8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1ffb8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1ffb8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ffb8-116">Not supported.</span></span>|
|<span data-ttu-id="1ffb8-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="1ffb8-117">Application</span></span>|<span data-ttu-id="1ffb8-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ffb8-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1ffb8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1ffb8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsWorkFromAnywhereMetrics/{userExperienceAnalyticsWorkFromAnywhereMetricId}/metricDevices/{userExperienceAnalyticsWorkFromAnywhereDeviceId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1ffb8-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1ffb8-120">Optional query parameters</span></span>
<span data-ttu-id="1ffb8-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1ffb8-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1ffb8-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1ffb8-122">Request headers</span></span>
|<span data-ttu-id="1ffb8-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1ffb8-123">Header</span></span>|<span data-ttu-id="1ffb8-124">Значение</span><span class="sxs-lookup"><span data-stu-id="1ffb8-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1ffb8-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1ffb8-125">Authorization</span></span>|<span data-ttu-id="1ffb8-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1ffb8-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1ffb8-127">Accept</span><span class="sxs-lookup"><span data-stu-id="1ffb8-127">Accept</span></span>|<span data-ttu-id="1ffb8-128">application/json</span><span class="sxs-lookup"><span data-stu-id="1ffb8-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ffb8-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1ffb8-129">Request body</span></span>
<span data-ttu-id="1ffb8-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1ffb8-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1ffb8-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="1ffb8-131">Response</span></span>
<span data-ttu-id="1ffb8-132">В случае успеха этот метод возвращает код отклика и `200 OK` [объект userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="1ffb8-132">If successful, this method returns a `200 OK` response code and [userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ffb8-133">Пример</span><span class="sxs-lookup"><span data-stu-id="1ffb8-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="1ffb8-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="1ffb8-134">Request</span></span>
<span data-ttu-id="1ffb8-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1ffb8-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsWorkFromAnywhereMetrics/{userExperienceAnalyticsWorkFromAnywhereMetricId}/metricDevices/{userExperienceAnalyticsWorkFromAnywhereDeviceId}
```

### <a name="response"></a><span data-ttu-id="1ffb8-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="1ffb8-136">Response</span></span>
<span data-ttu-id="1ffb8-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1ffb8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 599

{
  "value": {
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
}
```




