---
title: Get userExperienceAnalyticsMetricHistory
description: Чтение свойств и связей объекта userExperienceAnalyticsMetricHistory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3d2966b6298bda9453d9778a36bd7c89bc7f6d1a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50434981"
---
# <a name="get-userexperienceanalyticsmetrichistory"></a><span data-ttu-id="95cdc-103">Get userExperienceAnalyticsMetricHistory</span><span class="sxs-lookup"><span data-stu-id="95cdc-103">Get userExperienceAnalyticsMetricHistory</span></span>

<span data-ttu-id="95cdc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95cdc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="95cdc-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95cdc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95cdc-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="95cdc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95cdc-107">Чтение свойств и связей [объекта userExperienceAnalyticsMetricHistory.](../resources/intune-devices-userexperienceanalyticsmetrichistory.md)</span><span class="sxs-lookup"><span data-stu-id="95cdc-107">Read properties and relationships of the [userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="95cdc-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="95cdc-108">Prerequisites</span></span>
<span data-ttu-id="95cdc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95cdc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95cdc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="95cdc-111">Permission type</span></span>|<span data-ttu-id="95cdc-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="95cdc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="95cdc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="95cdc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="95cdc-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="95cdc-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="95cdc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="95cdc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95cdc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95cdc-116">Not supported.</span></span>|
|<span data-ttu-id="95cdc-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="95cdc-117">Application</span></span>|<span data-ttu-id="95cdc-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="95cdc-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="95cdc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="95cdc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsMetricHistory/{userExperienceAnalyticsMetricHistoryId}
GET /deviceManagement/userExperienceAnalyticsDeviceMetricHistory/{userExperienceAnalyticsMetricHistoryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="95cdc-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="95cdc-120">Optional query parameters</span></span>
<span data-ttu-id="95cdc-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="95cdc-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="95cdc-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="95cdc-122">Request headers</span></span>
|<span data-ttu-id="95cdc-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="95cdc-123">Header</span></span>|<span data-ttu-id="95cdc-124">Значение</span><span class="sxs-lookup"><span data-stu-id="95cdc-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="95cdc-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="95cdc-125">Authorization</span></span>|<span data-ttu-id="95cdc-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="95cdc-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="95cdc-127">Accept</span><span class="sxs-lookup"><span data-stu-id="95cdc-127">Accept</span></span>|<span data-ttu-id="95cdc-128">application/json</span><span class="sxs-lookup"><span data-stu-id="95cdc-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="95cdc-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="95cdc-129">Request body</span></span>
<span data-ttu-id="95cdc-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="95cdc-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="95cdc-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="95cdc-131">Response</span></span>
<span data-ttu-id="95cdc-132">В случае успеха этот метод возвращает код отклика и `200 OK` [объект userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="95cdc-132">If successful, this method returns a `200 OK` response code and [userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95cdc-133">Пример</span><span class="sxs-lookup"><span data-stu-id="95cdc-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="95cdc-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="95cdc-134">Request</span></span>
<span data-ttu-id="95cdc-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="95cdc-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsMetricHistory/{userExperienceAnalyticsMetricHistoryId}
```

### <a name="response"></a><span data-ttu-id="95cdc-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="95cdc-136">Response</span></span>
<span data-ttu-id="95cdc-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="95cdc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 286

{
  "value": {
    "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetricHistory",
    "id": "2b6d6456-6456-2b6d-5664-6d2b56646d2b",
    "deviceId": "Device Id value",
    "metricDateTime": "2017-01-01T00:00:28.4495993-08:00",
    "metricType": "Metric Type value"
  }
}
```




