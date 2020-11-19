---
title: Получение Усерекспериенцеаналитикскатегори
description: Чтение свойств и связей объекта Усерекспериенцеаналитикскатегори.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ab6c273a2aabfc306326005a1934f103b3b706cb
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49219050"
---
# <a name="get-userexperienceanalyticscategory"></a><span data-ttu-id="ec614-103">Получение Усерекспериенцеаналитикскатегори</span><span class="sxs-lookup"><span data-stu-id="ec614-103">Get userExperienceAnalyticsCategory</span></span>

<span data-ttu-id="ec614-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec614-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ec614-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec614-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ec614-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ec614-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec614-107">Чтение свойств и связей объекта [усерекспериенцеаналитикскатегори](../resources/intune-devices-userexperienceanalyticscategory.md) .</span><span class="sxs-lookup"><span data-stu-id="ec614-107">Read properties and relationships of the [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ec614-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ec614-108">Prerequisites</span></span>
<span data-ttu-id="ec614-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec614-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec614-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ec614-111">Permission type</span></span>|<span data-ttu-id="ec614-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ec614-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ec614-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ec614-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ec614-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="ec614-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="ec614-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ec614-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ec614-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec614-116">Not supported.</span></span>|
|<span data-ttu-id="ec614-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="ec614-117">Application</span></span>|<span data-ttu-id="ec614-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="ec614-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ec614-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ec614-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsAppHealthOverview
GET /deviceManagement/userExperienceAnalyticsCategories/{userExperienceAnalyticsCategoryId}
GET /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/bestPracticesMetrics
GET /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/rebootAnalyticsMetrics
GET /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/deviceBootPerformanceMetrics
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ec614-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ec614-120">Optional query parameters</span></span>
<span data-ttu-id="ec614-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ec614-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ec614-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ec614-122">Request headers</span></span>
|<span data-ttu-id="ec614-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ec614-123">Header</span></span>|<span data-ttu-id="ec614-124">Значение</span><span class="sxs-lookup"><span data-stu-id="ec614-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ec614-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ec614-125">Authorization</span></span>|<span data-ttu-id="ec614-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ec614-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ec614-127">Accept</span><span class="sxs-lookup"><span data-stu-id="ec614-127">Accept</span></span>|<span data-ttu-id="ec614-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ec614-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec614-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ec614-129">Request body</span></span>
<span data-ttu-id="ec614-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ec614-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ec614-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec614-131">Response</span></span>
<span data-ttu-id="ec614-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [усерекспериенцеаналитикскатегори](../resources/intune-devices-userexperienceanalyticscategory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ec614-132">If successful, this method returns a `200 OK` response code and [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec614-133">Пример</span><span class="sxs-lookup"><span data-stu-id="ec614-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="ec614-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="ec614-134">Request</span></span>
<span data-ttu-id="ec614-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ec614-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthOverview
```

### <a name="response"></a><span data-ttu-id="ec614-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec614-136">Response</span></span>
<span data-ttu-id="ec614-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ec614-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 657

{
  "value": {
    "@odata.type": "#microsoft.graph.userExperienceAnalyticsCategory",
    "id": "cfd28056-8056-cfd2-5680-d2cf5680d2cf",
    "overallScore": 12,
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
    "state": "insufficientData"
  }
}
```




