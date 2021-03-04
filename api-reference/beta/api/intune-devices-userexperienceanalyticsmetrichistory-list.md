---
title: Список userExperienceAnalyticsMetricHistories
description: Список свойств и связей объектов userExperienceAnalyticsMetricHistory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c6b5bd5a3675019fb673469f0071ef24bae2f699
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441524"
---
# <a name="list-userexperienceanalyticsmetrichistories"></a><span data-ttu-id="0bbc6-103">Список userExperienceAnalyticsMetricHistories</span><span class="sxs-lookup"><span data-stu-id="0bbc6-103">List userExperienceAnalyticsMetricHistories</span></span>

<span data-ttu-id="0bbc6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0bbc6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0bbc6-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0bbc6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0bbc6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0bbc6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0bbc6-107">Список свойств и связей [объектов userExperienceAnalyticsMetricHistory.](../resources/intune-devices-userexperienceanalyticsmetrichistory.md)</span><span class="sxs-lookup"><span data-stu-id="0bbc6-107">List properties and relationships of the [userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0bbc6-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0bbc6-108">Prerequisites</span></span>
<span data-ttu-id="0bbc6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0bbc6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0bbc6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0bbc6-111">Permission type</span></span>|<span data-ttu-id="0bbc6-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0bbc6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0bbc6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0bbc6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0bbc6-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="0bbc6-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="0bbc6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0bbc6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0bbc6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0bbc6-116">Not supported.</span></span>|
|<span data-ttu-id="0bbc6-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="0bbc6-117">Application</span></span>|<span data-ttu-id="0bbc6-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="0bbc6-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0bbc6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0bbc6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsMetricHistory
GET /deviceManagement/userExperienceAnalyticsDeviceMetricHistory
```

## <a name="request-headers"></a><span data-ttu-id="0bbc6-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0bbc6-120">Request headers</span></span>
|<span data-ttu-id="0bbc6-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0bbc6-121">Header</span></span>|<span data-ttu-id="0bbc6-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0bbc6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0bbc6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0bbc6-123">Authorization</span></span>|<span data-ttu-id="0bbc6-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0bbc6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0bbc6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0bbc6-125">Accept</span></span>|<span data-ttu-id="0bbc6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0bbc6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0bbc6-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0bbc6-127">Request body</span></span>
<span data-ttu-id="0bbc6-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0bbc6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0bbc6-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="0bbc6-129">Response</span></span>
<span data-ttu-id="0bbc6-130">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="0bbc6-130">If successful, this method returns a `200 OK` response code and a collection of [userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0bbc6-131">Пример</span><span class="sxs-lookup"><span data-stu-id="0bbc6-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="0bbc6-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="0bbc6-132">Request</span></span>
<span data-ttu-id="0bbc6-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0bbc6-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsMetricHistory
```

### <a name="response"></a><span data-ttu-id="0bbc6-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="0bbc6-134">Response</span></span>
<span data-ttu-id="0bbc6-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0bbc6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 310

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetricHistory",
      "id": "2b6d6456-6456-2b6d-5664-6d2b56646d2b",
      "deviceId": "Device Id value",
      "metricDateTime": "2017-01-01T00:00:28.4495993-08:00",
      "metricType": "Metric Type value"
    }
  ]
}
```




