---
title: Get userExperienceAnalyticsOverview
description: Чтение свойств и связей объекта userExperienceAnalyticsOverview.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ae30966ec42edc00dc4245fb9f8b58ad85461346
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51159160"
---
# <a name="get-userexperienceanalyticsoverview"></a><span data-ttu-id="cbb12-103">Get userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="cbb12-103">Get userExperienceAnalyticsOverview</span></span>

<span data-ttu-id="cbb12-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cbb12-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cbb12-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cbb12-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cbb12-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cbb12-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cbb12-107">Чтение свойств и связей [объекта userExperienceAnalyticsOverview.](../resources/intune-devices-userexperienceanalyticsoverview.md)</span><span class="sxs-lookup"><span data-stu-id="cbb12-107">Read properties and relationships of the [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cbb12-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="cbb12-108">Prerequisites</span></span>
<span data-ttu-id="cbb12-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cbb12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cbb12-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cbb12-111">Permission type</span></span>|<span data-ttu-id="cbb12-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cbb12-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cbb12-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cbb12-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cbb12-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cbb12-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="cbb12-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cbb12-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cbb12-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cbb12-116">Not supported.</span></span>|
|<span data-ttu-id="cbb12-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="cbb12-117">Application</span></span>|<span data-ttu-id="cbb12-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cbb12-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cbb12-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cbb12-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cbb12-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cbb12-120">Optional query parameters</span></span>
<span data-ttu-id="cbb12-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="cbb12-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cbb12-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cbb12-122">Request headers</span></span>
|<span data-ttu-id="cbb12-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cbb12-123">Header</span></span>|<span data-ttu-id="cbb12-124">Значение</span><span class="sxs-lookup"><span data-stu-id="cbb12-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cbb12-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="cbb12-125">Authorization</span></span>|<span data-ttu-id="cbb12-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cbb12-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cbb12-127">Accept</span><span class="sxs-lookup"><span data-stu-id="cbb12-127">Accept</span></span>|<span data-ttu-id="cbb12-128">application/json</span><span class="sxs-lookup"><span data-stu-id="cbb12-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cbb12-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cbb12-129">Request body</span></span>
<span data-ttu-id="cbb12-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cbb12-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cbb12-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="cbb12-131">Response</span></span>
<span data-ttu-id="cbb12-132">В случае успеха этот метод возвращает код отклика и `200 OK` [объект userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="cbb12-132">If successful, this method returns a `200 OK` response code and [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cbb12-133">Пример</span><span class="sxs-lookup"><span data-stu-id="cbb12-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="cbb12-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="cbb12-134">Request</span></span>
<span data-ttu-id="cbb12-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cbb12-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsOverview
```

### <a name="response"></a><span data-ttu-id="cbb12-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="cbb12-136">Response</span></span>
<span data-ttu-id="cbb12-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cbb12-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1123

{
  "value": {
    "@odata.type": "#microsoft.graph.userExperienceAnalyticsOverview",
    "id": "8228da2b-da2b-8228-2bda-28822bda2882",
    "overallScore": 12,
    "deviceBootPerformanceOverallScore": 1,
    "bestPracticesOverallScore": 9,
    "workFromAnywhereOverallScore": 12,
    "appHealthOverallScore": 5,
    "resourcePerformanceOverallScore": 15,
    "insights": [
      {
        "@odata.type": "microsoft.graph.userExperienceAnalyticsInsight",
        "userExperienceAnalyticsMetricId": "User Experience Analytics Metric Id value",
        "insightId": "Insight Id value",
        "values": [
          {
            "@odata.type": "microsoft.graph.insightValueDouble",
            "value": 1.6666666666666667
          }
        ],
        "severity": "informational"
      }
    ],
    "state": "insufficientData",
    "deviceBootPerformanceHealthState": "insufficientData",
    "bestPracticesHealthState": "insufficientData",
    "workFromAnywhereHealthState": "insufficientData",
    "appHealthState": "insufficientData",
    "resourcePerformanceState": "insufficientData"
  }
}
```




