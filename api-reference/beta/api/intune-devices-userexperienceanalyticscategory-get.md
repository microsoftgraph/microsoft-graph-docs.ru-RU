---
title: Получение Усерекспериенцеаналитикскатегори
description: Чтение свойств и связей объекта Усерекспериенцеаналитикскатегори.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e8a499b5a9d82b441510038b2703b1f560379684
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36311729"
---
# <a name="get-userexperienceanalyticscategory"></a><span data-ttu-id="f5f94-103">Получение Усерекспериенцеаналитикскатегори</span><span class="sxs-lookup"><span data-stu-id="f5f94-103">Get userExperienceAnalyticsCategory</span></span>

> <span data-ttu-id="f5f94-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5f94-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f5f94-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f5f94-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f5f94-106">Чтение свойств и связей объекта [усерекспериенцеаналитикскатегори](../resources/intune-devices-userexperienceanalyticscategory.md) .</span><span class="sxs-lookup"><span data-stu-id="f5f94-106">Read properties and relationships of the [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f5f94-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f5f94-107">Prerequisites</span></span>
<span data-ttu-id="f5f94-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5f94-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5f94-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f5f94-110">Permission type</span></span>|<span data-ttu-id="f5f94-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f5f94-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f5f94-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f5f94-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f5f94-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="f5f94-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="f5f94-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f5f94-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f5f94-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5f94-115">Not supported.</span></span>|
|<span data-ttu-id="f5f94-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f5f94-116">Application</span></span>|<span data-ttu-id="f5f94-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="f5f94-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f5f94-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f5f94-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsCategories/{userExperienceAnalyticsCategoryId}
GET /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/bestPracticesMetrics
GET /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/deviceBootPerformanceMetrics
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f5f94-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f5f94-119">Optional query parameters</span></span>
<span data-ttu-id="f5f94-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f5f94-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f5f94-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f5f94-121">Request headers</span></span>
|<span data-ttu-id="f5f94-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f5f94-122">Header</span></span>|<span data-ttu-id="f5f94-123">Значение</span><span class="sxs-lookup"><span data-stu-id="f5f94-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f5f94-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f5f94-124">Authorization</span></span>|<span data-ttu-id="f5f94-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f5f94-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f5f94-126">Accept</span><span class="sxs-lookup"><span data-stu-id="f5f94-126">Accept</span></span>|<span data-ttu-id="f5f94-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f5f94-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5f94-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f5f94-128">Request body</span></span>
<span data-ttu-id="f5f94-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f5f94-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f5f94-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="f5f94-130">Response</span></span>
<span data-ttu-id="f5f94-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [усерекспериенцеаналитикскатегори](../resources/intune-devices-userexperienceanalyticscategory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f5f94-131">If successful, this method returns a `200 OK` response code and [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5f94-132">Пример</span><span class="sxs-lookup"><span data-stu-id="f5f94-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="f5f94-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="f5f94-133">Request</span></span>
<span data-ttu-id="f5f94-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f5f94-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsCategories/{userExperienceAnalyticsCategoryId}
```

### <a name="response"></a><span data-ttu-id="f5f94-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="f5f94-135">Response</span></span>
<span data-ttu-id="f5f94-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f5f94-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 584

{
  "value": {
    "@odata.type": "#microsoft.graph.userExperienceAnalyticsCategory",
    "id": "cfd28056-8056-cfd2-5680-d2cf5680d2cf",
    "displayName": "Display Name value",
    "overallScore": 12,
    "insights": [
      {
        "@odata.type": "microsoft.graph.userExperienceAnalyticsInsight",
        "userExperienceAnalyticsMetricId": "User Experience Analytics Metric Id value",
        "insightId": "Insight Id value",
        "value": [
          {
            "@odata.type": "microsoft.graph.insightValueDouble"
          }
        ]
      }
    ]
  }
}
```






