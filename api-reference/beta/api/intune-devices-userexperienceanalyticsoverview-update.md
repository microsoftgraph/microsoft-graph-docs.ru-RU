---
title: Обновление userExperienceAnalyticsOverview
description: Обновление свойств объекта userExperienceAnalyticsOverview.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 02383cd8ac10d7c383b3cd84c25d4dc57c9bd71b
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50434967"
---
# <a name="update-userexperienceanalyticsoverview"></a><span data-ttu-id="097ab-103">Обновление userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="097ab-103">Update userExperienceAnalyticsOverview</span></span>

<span data-ttu-id="097ab-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="097ab-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="097ab-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="097ab-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="097ab-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="097ab-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="097ab-107">Обновление свойств объекта [userExperienceAnalyticsOverview.](../resources/intune-devices-userexperienceanalyticsoverview.md)</span><span class="sxs-lookup"><span data-stu-id="097ab-107">Update the properties of a [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="097ab-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="097ab-108">Prerequisites</span></span>
<span data-ttu-id="097ab-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="097ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="097ab-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="097ab-111">Permission type</span></span>|<span data-ttu-id="097ab-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="097ab-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="097ab-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="097ab-113">Delegated (work or school account)</span></span>|<span data-ttu-id="097ab-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="097ab-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="097ab-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="097ab-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="097ab-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="097ab-116">Not supported.</span></span>|
|<span data-ttu-id="097ab-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="097ab-117">Application</span></span>|<span data-ttu-id="097ab-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="097ab-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="097ab-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="097ab-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsOverview
```

## <a name="request-headers"></a><span data-ttu-id="097ab-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="097ab-120">Request headers</span></span>
|<span data-ttu-id="097ab-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="097ab-121">Header</span></span>|<span data-ttu-id="097ab-122">Значение</span><span class="sxs-lookup"><span data-stu-id="097ab-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="097ab-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="097ab-123">Authorization</span></span>|<span data-ttu-id="097ab-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="097ab-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="097ab-125">Accept</span><span class="sxs-lookup"><span data-stu-id="097ab-125">Accept</span></span>|<span data-ttu-id="097ab-126">application/json</span><span class="sxs-lookup"><span data-stu-id="097ab-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="097ab-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="097ab-127">Request body</span></span>
<span data-ttu-id="097ab-128">В теле запроса поставляем представление JSON для [объекта userExperienceAnalyticsOverview.](../resources/intune-devices-userexperienceanalyticsoverview.md)</span><span class="sxs-lookup"><span data-stu-id="097ab-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>

<span data-ttu-id="097ab-129">В следующей таблице показаны свойства, необходимые при создании [userExperienceAnalyticsOverview.](../resources/intune-devices-userexperienceanalyticsoverview.md)</span><span class="sxs-lookup"><span data-stu-id="097ab-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md).</span></span>

|<span data-ttu-id="097ab-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="097ab-130">Property</span></span>|<span data-ttu-id="097ab-131">Тип</span><span class="sxs-lookup"><span data-stu-id="097ab-131">Type</span></span>|<span data-ttu-id="097ab-132">Описание</span><span class="sxs-lookup"><span data-stu-id="097ab-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="097ab-133">id</span><span class="sxs-lookup"><span data-stu-id="097ab-133">id</span></span>|<span data-ttu-id="097ab-134">String</span><span class="sxs-lookup"><span data-stu-id="097ab-134">String</span></span>|<span data-ttu-id="097ab-135">Уникальный идентификатор обзора аналитики пользовательских интерфейсов.</span><span class="sxs-lookup"><span data-stu-id="097ab-135">The unique identifier of the user experience analytics overview.</span></span>|
|<span data-ttu-id="097ab-136">overallScore</span><span class="sxs-lookup"><span data-stu-id="097ab-136">overallScore</span></span>|<span data-ttu-id="097ab-137">Int32</span><span class="sxs-lookup"><span data-stu-id="097ab-137">Int32</span></span>|<span data-ttu-id="097ab-138">Общая оценка аналитики пользовательского опыта.</span><span class="sxs-lookup"><span data-stu-id="097ab-138">The user experience analytics overall score.</span></span>|
|<span data-ttu-id="097ab-139">deviceBootPerformanceOverallScore</span><span class="sxs-lookup"><span data-stu-id="097ab-139">deviceBootPerformanceOverallScore</span></span>|<span data-ttu-id="097ab-140">Int32</span><span class="sxs-lookup"><span data-stu-id="097ab-140">Int32</span></span>|<span data-ttu-id="097ab-141">Общая оценка производительности загрузки устройства для аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="097ab-141">The user experience analytics device boot performance overall score.</span></span>|
|<span data-ttu-id="097ab-142">bestPracticesOverallScore</span><span class="sxs-lookup"><span data-stu-id="097ab-142">bestPracticesOverallScore</span></span>|<span data-ttu-id="097ab-143">Int32</span><span class="sxs-lookup"><span data-stu-id="097ab-143">Int32</span></span>|<span data-ttu-id="097ab-144">Анализ пользовательских интерфейсов позволяет опытом работы с общим показателем.</span><span class="sxs-lookup"><span data-stu-id="097ab-144">The user experience analytics best practices overall score.</span></span>|
|<span data-ttu-id="097ab-145">appHealthOverallScore</span><span class="sxs-lookup"><span data-stu-id="097ab-145">appHealthOverallScore</span></span>|<span data-ttu-id="097ab-146">Int32</span><span class="sxs-lookup"><span data-stu-id="097ab-146">Int32</span></span>|<span data-ttu-id="097ab-147">Общее состояние здоровья приложения для аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="097ab-147">The user experience analytics app health overall score.</span></span>|
|<span data-ttu-id="097ab-148">resourcePerformanceOverallScore</span><span class="sxs-lookup"><span data-stu-id="097ab-148">resourcePerformanceOverallScore</span></span>|<span data-ttu-id="097ab-149">Int32</span><span class="sxs-lookup"><span data-stu-id="097ab-149">Int32</span></span>|<span data-ttu-id="097ab-150">Общая оценка производительности ресурсов аналитики пользовательских ресурсов.</span><span class="sxs-lookup"><span data-stu-id="097ab-150">The user experience analytics resource performance overall score.</span></span>|
|<span data-ttu-id="097ab-151">insights</span><span class="sxs-lookup"><span data-stu-id="097ab-151">insights</span></span>|<span data-ttu-id="097ab-152">[коллекция userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md)</span><span class="sxs-lookup"><span data-stu-id="097ab-152">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="097ab-153">Аналитические сведения о пользовательском опыте.</span><span class="sxs-lookup"><span data-stu-id="097ab-153">The user experience analytics insights.</span></span>|
|<span data-ttu-id="097ab-154">state</span><span class="sxs-lookup"><span data-stu-id="097ab-154">state</span></span>|[<span data-ttu-id="097ab-155">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="097ab-155">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="097ab-156">Текущее состояние состояния состояния аналитики пользовательских интерфейсов.</span><span class="sxs-lookup"><span data-stu-id="097ab-156">The current health state of the user experience analytics overview.</span></span> <span data-ttu-id="097ab-157">Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="097ab-157">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="097ab-158">deviceBootPerformanceHealthState</span><span class="sxs-lookup"><span data-stu-id="097ab-158">deviceBootPerformanceHealthState</span></span>|[<span data-ttu-id="097ab-159">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="097ab-159">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="097ab-160">Текущее состояние состояния состояния аналитики пользовательского интерфейса категории BootPerformance.</span><span class="sxs-lookup"><span data-stu-id="097ab-160">The current health state of the user experience analytics 'BootPerformance' category.</span></span> <span data-ttu-id="097ab-161">Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="097ab-161">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="097ab-162">bestPracticesHealthState</span><span class="sxs-lookup"><span data-stu-id="097ab-162">bestPracticesHealthState</span></span>|[<span data-ttu-id="097ab-163">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="097ab-163">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="097ab-164">Текущее состояние здоровья категории аналитики пользовательских интерфейсов "BestPractices".</span><span class="sxs-lookup"><span data-stu-id="097ab-164">The current health state of the user experience analytics 'BestPractices' category.</span></span> <span data-ttu-id="097ab-165">Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="097ab-165">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="097ab-166">appHealthState</span><span class="sxs-lookup"><span data-stu-id="097ab-166">appHealthState</span></span>|[<span data-ttu-id="097ab-167">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="097ab-167">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="097ab-168">Текущее состояние здоровья категории аналитики пользовательских интерфейсов "BestPractices".</span><span class="sxs-lookup"><span data-stu-id="097ab-168">The current health state of the user experience analytics 'BestPractices' category.</span></span> <span data-ttu-id="097ab-169">Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="097ab-169">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="097ab-170">resourcePerformanceState</span><span class="sxs-lookup"><span data-stu-id="097ab-170">resourcePerformanceState</span></span>|[<span data-ttu-id="097ab-171">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="097ab-171">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="097ab-172">Текущее состояние состояния здоровья в категории аналитики пользовательского интерфейса "ResourcePerformance".</span><span class="sxs-lookup"><span data-stu-id="097ab-172">The current health state of the user experience analytics 'ResourcePerformance' category.</span></span> <span data-ttu-id="097ab-173">Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="097ab-173">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|



## <a name="response"></a><span data-ttu-id="097ab-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="097ab-174">Response</span></span>
<span data-ttu-id="097ab-175">В случае успеха этот метод возвращает код отклика и обновленный `200 OK` [объект userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="097ab-175">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="097ab-176">Пример</span><span class="sxs-lookup"><span data-stu-id="097ab-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="097ab-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="097ab-177">Request</span></span>
<span data-ttu-id="097ab-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="097ab-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsOverview
Content-type: application/json
Content-length: 906

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsOverview",
  "overallScore": 12,
  "deviceBootPerformanceOverallScore": 1,
  "bestPracticesOverallScore": 9,
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
  "appHealthState": "insufficientData",
  "resourcePerformanceState": "insufficientData"
}
```

### <a name="response"></a><span data-ttu-id="097ab-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="097ab-179">Response</span></span>
<span data-ttu-id="097ab-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="097ab-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 955

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsOverview",
  "id": "8228da2b-da2b-8228-2bda-28822bda2882",
  "overallScore": 12,
  "deviceBootPerformanceOverallScore": 1,
  "bestPracticesOverallScore": 9,
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
  "appHealthState": "insufficientData",
  "resourcePerformanceState": "insufficientData"
}
```




