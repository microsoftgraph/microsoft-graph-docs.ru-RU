---
title: Обновление userExperienceAnalyticsOverview
description: Обновление свойств объекта userExperienceAnalyticsOverview.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: dbe91b8e131e4379c8d658cea6420aad9fbf2c9e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51149977"
---
# <a name="update-userexperienceanalyticsoverview"></a><span data-ttu-id="24c5d-103">Обновление userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="24c5d-103">Update userExperienceAnalyticsOverview</span></span>

<span data-ttu-id="24c5d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24c5d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="24c5d-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24c5d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24c5d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="24c5d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24c5d-107">Обновление свойств объекта [userExperienceAnalyticsOverview.](../resources/intune-devices-userexperienceanalyticsoverview.md)</span><span class="sxs-lookup"><span data-stu-id="24c5d-107">Update the properties of a [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="24c5d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="24c5d-108">Prerequisites</span></span>
<span data-ttu-id="24c5d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24c5d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24c5d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="24c5d-111">Permission type</span></span>|<span data-ttu-id="24c5d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="24c5d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24c5d-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="24c5d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="24c5d-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24c5d-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="24c5d-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="24c5d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24c5d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24c5d-116">Not supported.</span></span>|
|<span data-ttu-id="24c5d-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="24c5d-117">Application</span></span>|<span data-ttu-id="24c5d-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24c5d-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="24c5d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="24c5d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsOverview
```

## <a name="request-headers"></a><span data-ttu-id="24c5d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="24c5d-120">Request headers</span></span>
|<span data-ttu-id="24c5d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="24c5d-121">Header</span></span>|<span data-ttu-id="24c5d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="24c5d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="24c5d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="24c5d-123">Authorization</span></span>|<span data-ttu-id="24c5d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="24c5d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="24c5d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="24c5d-125">Accept</span></span>|<span data-ttu-id="24c5d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="24c5d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="24c5d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="24c5d-127">Request body</span></span>
<span data-ttu-id="24c5d-128">В теле запроса поставляем представление JSON для [объекта userExperienceAnalyticsOverview.](../resources/intune-devices-userexperienceanalyticsoverview.md)</span><span class="sxs-lookup"><span data-stu-id="24c5d-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>

<span data-ttu-id="24c5d-129">В следующей таблице показаны свойства, необходимые при создании [userExperienceAnalyticsOverview.](../resources/intune-devices-userexperienceanalyticsoverview.md)</span><span class="sxs-lookup"><span data-stu-id="24c5d-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md).</span></span>

|<span data-ttu-id="24c5d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="24c5d-130">Property</span></span>|<span data-ttu-id="24c5d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="24c5d-131">Type</span></span>|<span data-ttu-id="24c5d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="24c5d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24c5d-133">id</span><span class="sxs-lookup"><span data-stu-id="24c5d-133">id</span></span>|<span data-ttu-id="24c5d-134">Строка</span><span class="sxs-lookup"><span data-stu-id="24c5d-134">String</span></span>|<span data-ttu-id="24c5d-135">Уникальный идентификатор обзора аналитики пользовательских интерфейсов.</span><span class="sxs-lookup"><span data-stu-id="24c5d-135">The unique identifier of the user experience analytics overview.</span></span>|
|<span data-ttu-id="24c5d-136">overallScore</span><span class="sxs-lookup"><span data-stu-id="24c5d-136">overallScore</span></span>|<span data-ttu-id="24c5d-137">Int32</span><span class="sxs-lookup"><span data-stu-id="24c5d-137">Int32</span></span>|<span data-ttu-id="24c5d-138">Общая оценка аналитики пользовательского опыта.</span><span class="sxs-lookup"><span data-stu-id="24c5d-138">The user experience analytics overall score.</span></span>|
|<span data-ttu-id="24c5d-139">deviceBootPerformanceOverallScore</span><span class="sxs-lookup"><span data-stu-id="24c5d-139">deviceBootPerformanceOverallScore</span></span>|<span data-ttu-id="24c5d-140">Int32</span><span class="sxs-lookup"><span data-stu-id="24c5d-140">Int32</span></span>|<span data-ttu-id="24c5d-141">Общая оценка производительности загрузки устройства для аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="24c5d-141">The user experience analytics device boot performance overall score.</span></span>|
|<span data-ttu-id="24c5d-142">bestPracticesOverallScore</span><span class="sxs-lookup"><span data-stu-id="24c5d-142">bestPracticesOverallScore</span></span>|<span data-ttu-id="24c5d-143">Int32</span><span class="sxs-lookup"><span data-stu-id="24c5d-143">Int32</span></span>|<span data-ttu-id="24c5d-144">Анализ пользовательских интерфейсов позволяет опытом работы с общим показателем.</span><span class="sxs-lookup"><span data-stu-id="24c5d-144">The user experience analytics best practices overall score.</span></span>|
|<span data-ttu-id="24c5d-145">workFromAnywhereOverallScore</span><span class="sxs-lookup"><span data-stu-id="24c5d-145">workFromAnywhereOverallScore</span></span>|<span data-ttu-id="24c5d-146">Int32</span><span class="sxs-lookup"><span data-stu-id="24c5d-146">Int32</span></span>|<span data-ttu-id="24c5d-147">Аналитика пользовательского интерфейса Работает с любого общего балла.</span><span class="sxs-lookup"><span data-stu-id="24c5d-147">The user experience analytics Work From Anywhere overall score.</span></span>|
|<span data-ttu-id="24c5d-148">appHealthOverallScore</span><span class="sxs-lookup"><span data-stu-id="24c5d-148">appHealthOverallScore</span></span>|<span data-ttu-id="24c5d-149">Int32</span><span class="sxs-lookup"><span data-stu-id="24c5d-149">Int32</span></span>|<span data-ttu-id="24c5d-150">Общее состояние здоровья приложения для аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="24c5d-150">The user experience analytics app health overall score.</span></span>|
|<span data-ttu-id="24c5d-151">resourcePerformanceOverallScore</span><span class="sxs-lookup"><span data-stu-id="24c5d-151">resourcePerformanceOverallScore</span></span>|<span data-ttu-id="24c5d-152">Int32</span><span class="sxs-lookup"><span data-stu-id="24c5d-152">Int32</span></span>|<span data-ttu-id="24c5d-153">Общая оценка производительности ресурсов аналитики пользовательских ресурсов.</span><span class="sxs-lookup"><span data-stu-id="24c5d-153">The user experience analytics resource performance overall score.</span></span>|
|<span data-ttu-id="24c5d-154">insights</span><span class="sxs-lookup"><span data-stu-id="24c5d-154">insights</span></span>|<span data-ttu-id="24c5d-155">[коллекция userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md)</span><span class="sxs-lookup"><span data-stu-id="24c5d-155">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="24c5d-156">Аналитические сведения о пользовательском опыте.</span><span class="sxs-lookup"><span data-stu-id="24c5d-156">The user experience analytics insights.</span></span>|
|<span data-ttu-id="24c5d-157">state</span><span class="sxs-lookup"><span data-stu-id="24c5d-157">state</span></span>|[<span data-ttu-id="24c5d-158">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="24c5d-158">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="24c5d-159">Текущее состояние состояния состояния аналитики пользовательских интерфейсов.</span><span class="sxs-lookup"><span data-stu-id="24c5d-159">The current health state of the user experience analytics overview.</span></span> <span data-ttu-id="24c5d-160">Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="24c5d-160">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="24c5d-161">deviceBootPerformanceHealthState</span><span class="sxs-lookup"><span data-stu-id="24c5d-161">deviceBootPerformanceHealthState</span></span>|[<span data-ttu-id="24c5d-162">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="24c5d-162">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="24c5d-163">Текущее состояние состояния состояния аналитики пользовательского интерфейса категории BootPerformance.</span><span class="sxs-lookup"><span data-stu-id="24c5d-163">The current health state of the user experience analytics 'BootPerformance' category.</span></span> <span data-ttu-id="24c5d-164">Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="24c5d-164">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="24c5d-165">bestPracticesHealthState</span><span class="sxs-lookup"><span data-stu-id="24c5d-165">bestPracticesHealthState</span></span>|[<span data-ttu-id="24c5d-166">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="24c5d-166">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="24c5d-167">Текущее состояние здоровья категории аналитики пользовательских интерфейсов "BestPractices".</span><span class="sxs-lookup"><span data-stu-id="24c5d-167">The current health state of the user experience analytics 'BestPractices' category.</span></span> <span data-ttu-id="24c5d-168">Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="24c5d-168">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="24c5d-169">workFromAnywhereHealthState</span><span class="sxs-lookup"><span data-stu-id="24c5d-169">workFromAnywhereHealthState</span></span>|[<span data-ttu-id="24c5d-170">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="24c5d-170">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="24c5d-171">Текущее состояние состояния здоровья аналитики пользовательских интерфейсов категории WorkFromAnywhere.</span><span class="sxs-lookup"><span data-stu-id="24c5d-171">The current health state of the user experience analytics 'WorkFromAnywhere' category.</span></span> <span data-ttu-id="24c5d-172">Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="24c5d-172">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="24c5d-173">appHealthState</span><span class="sxs-lookup"><span data-stu-id="24c5d-173">appHealthState</span></span>|[<span data-ttu-id="24c5d-174">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="24c5d-174">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="24c5d-175">Текущее состояние здоровья категории аналитики пользовательских интерфейсов "BestPractices".</span><span class="sxs-lookup"><span data-stu-id="24c5d-175">The current health state of the user experience analytics 'BestPractices' category.</span></span> <span data-ttu-id="24c5d-176">Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="24c5d-176">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="24c5d-177">resourcePerformanceState</span><span class="sxs-lookup"><span data-stu-id="24c5d-177">resourcePerformanceState</span></span>|[<span data-ttu-id="24c5d-178">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="24c5d-178">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="24c5d-179">Текущее состояние состояния здоровья в категории аналитики пользовательского интерфейса "ResourcePerformance".</span><span class="sxs-lookup"><span data-stu-id="24c5d-179">The current health state of the user experience analytics 'ResourcePerformance' category.</span></span> <span data-ttu-id="24c5d-180">Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="24c5d-180">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|



## <a name="response"></a><span data-ttu-id="24c5d-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="24c5d-181">Response</span></span>
<span data-ttu-id="24c5d-182">В случае успеха этот метод возвращает код отклика и обновленный `200 OK` [объект userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="24c5d-182">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24c5d-183">Пример</span><span class="sxs-lookup"><span data-stu-id="24c5d-183">Example</span></span>

### <a name="request"></a><span data-ttu-id="24c5d-184">Запрос</span><span class="sxs-lookup"><span data-stu-id="24c5d-184">Request</span></span>
<span data-ttu-id="24c5d-185">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="24c5d-185">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsOverview
Content-type: application/json
Content-length: 999

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsOverview",
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
```

### <a name="response"></a><span data-ttu-id="24c5d-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="24c5d-186">Response</span></span>
<span data-ttu-id="24c5d-p108">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="24c5d-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1048

{
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
```




