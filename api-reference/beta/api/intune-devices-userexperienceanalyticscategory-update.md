---
title: Обновление userExperienceAnalyticsCategory
description: Обновление свойств объекта userExperienceAnalyticsCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7d2529e8bb6d07ec45dc7bee675594b10a02d696
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155078"
---
# <a name="update-userexperienceanalyticscategory"></a><span data-ttu-id="42944-103">Обновление userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="42944-103">Update userExperienceAnalyticsCategory</span></span>

<span data-ttu-id="42944-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42944-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="42944-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42944-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="42944-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="42944-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42944-107">Обновление свойств объекта [userExperienceAnalyticsCategory.](../resources/intune-devices-userexperienceanalyticscategory.md)</span><span class="sxs-lookup"><span data-stu-id="42944-107">Update the properties of a [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="42944-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="42944-108">Prerequisites</span></span>
<span data-ttu-id="42944-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42944-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42944-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="42944-111">Permission type</span></span>|<span data-ttu-id="42944-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="42944-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="42944-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="42944-113">Delegated (work or school account)</span></span>|<span data-ttu-id="42944-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42944-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="42944-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="42944-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42944-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42944-116">Not supported.</span></span>|
|<span data-ttu-id="42944-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="42944-117">Application</span></span>|<span data-ttu-id="42944-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42944-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="42944-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="42944-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsAppHealthOverview
PATCH /deviceManagement/userExperienceAnalyticsCategories/{userExperienceAnalyticsCategoryId}
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/appHealthMetrics
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/bestPracticesMetrics
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/rebootAnalyticsMetrics
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/resourcePerformanceMetrics
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/deviceBootPerformanceMetrics
```

## <a name="request-headers"></a><span data-ttu-id="42944-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="42944-120">Request headers</span></span>
|<span data-ttu-id="42944-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="42944-121">Header</span></span>|<span data-ttu-id="42944-122">Значение</span><span class="sxs-lookup"><span data-stu-id="42944-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="42944-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="42944-123">Authorization</span></span>|<span data-ttu-id="42944-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="42944-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="42944-125">Accept</span><span class="sxs-lookup"><span data-stu-id="42944-125">Accept</span></span>|<span data-ttu-id="42944-126">application/json</span><span class="sxs-lookup"><span data-stu-id="42944-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="42944-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="42944-127">Request body</span></span>
<span data-ttu-id="42944-128">В теле запроса укажу представление объекта [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="42944-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>

<span data-ttu-id="42944-129">В следующей таблице показаны свойства, необходимые при создании [объекта userExperienceAnalyticsCategory.](../resources/intune-devices-userexperienceanalyticscategory.md)</span><span class="sxs-lookup"><span data-stu-id="42944-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md).</span></span>

|<span data-ttu-id="42944-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="42944-130">Property</span></span>|<span data-ttu-id="42944-131">Тип</span><span class="sxs-lookup"><span data-stu-id="42944-131">Type</span></span>|<span data-ttu-id="42944-132">Описание</span><span class="sxs-lookup"><span data-stu-id="42944-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42944-133">id</span><span class="sxs-lookup"><span data-stu-id="42944-133">id</span></span>|<span data-ttu-id="42944-134">String</span><span class="sxs-lookup"><span data-stu-id="42944-134">String</span></span>|<span data-ttu-id="42944-135">Уникальный идентификатор категории аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="42944-135">The unique identifier of the user experience analytics category.</span></span>|
|<span data-ttu-id="42944-136">overallScore</span><span class="sxs-lookup"><span data-stu-id="42944-136">overallScore</span></span>|<span data-ttu-id="42944-137">Int32</span><span class="sxs-lookup"><span data-stu-id="42944-137">Int32</span></span>|<span data-ttu-id="42944-138">Общая оценка категории аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="42944-138">The overall score of the user experience analytics category.</span></span>|
|<span data-ttu-id="42944-139">insights</span><span class="sxs-lookup"><span data-stu-id="42944-139">insights</span></span>|<span data-ttu-id="42944-140">[Коллекция userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md)</span><span class="sxs-lookup"><span data-stu-id="42944-140">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="42944-141">Аналитика для категории аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="42944-141">The insights for the user experience analytics category.</span></span>|
|<span data-ttu-id="42944-142">state</span><span class="sxs-lookup"><span data-stu-id="42944-142">state</span></span>|[<span data-ttu-id="42944-143">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="42944-143">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="42944-144">Текущее состояние состояния категории аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="42944-144">The current health state of the user experience analytics category.</span></span> <span data-ttu-id="42944-145">Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="42944-145">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|



## <a name="response"></a><span data-ttu-id="42944-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="42944-146">Response</span></span>
<span data-ttu-id="42944-147">В случае успеха этот метод возвращает код отклика и обновленный объект `200 OK` [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="42944-147">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42944-148">Пример</span><span class="sxs-lookup"><span data-stu-id="42944-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="42944-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="42944-149">Request</span></span>
<span data-ttu-id="42944-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="42944-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthOverview
Content-type: application/json
Content-length: 553

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsCategory",
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
```

### <a name="response"></a><span data-ttu-id="42944-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="42944-151">Response</span></span>
<span data-ttu-id="42944-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="42944-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 602

{
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
```




