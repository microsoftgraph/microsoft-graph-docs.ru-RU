---
title: Обновление userExperienceAnalyticsOverview
description: Обновление свойств объекта userExperienceAnalyticsOverview.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c1df141edc551b62aea8c32534aa852490d9772f
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866708"
---
# <a name="update-userexperienceanalyticsoverview"></a><span data-ttu-id="6765b-103">Обновление userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="6765b-103">Update userExperienceAnalyticsOverview</span></span>

<span data-ttu-id="6765b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6765b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6765b-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6765b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6765b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6765b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6765b-107">Обновление свойств объекта [userExperienceAnalyticsOverview.](../resources/intune-devices-userexperienceanalyticsoverview.md)</span><span class="sxs-lookup"><span data-stu-id="6765b-107">Update the properties of a [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6765b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6765b-108">Prerequisites</span></span>
<span data-ttu-id="6765b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6765b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6765b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6765b-111">Permission type</span></span>|<span data-ttu-id="6765b-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6765b-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6765b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6765b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6765b-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6765b-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="6765b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6765b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6765b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6765b-116">Not supported.</span></span>|
|<span data-ttu-id="6765b-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="6765b-117">Application</span></span>|<span data-ttu-id="6765b-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6765b-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6765b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6765b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsOverview
```

## <a name="request-headers"></a><span data-ttu-id="6765b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6765b-120">Request headers</span></span>
|<span data-ttu-id="6765b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6765b-121">Header</span></span>|<span data-ttu-id="6765b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6765b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6765b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6765b-123">Authorization</span></span>|<span data-ttu-id="6765b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6765b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6765b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6765b-125">Accept</span></span>|<span data-ttu-id="6765b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6765b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6765b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6765b-127">Request body</span></span>
<span data-ttu-id="6765b-128">В теле запроса поставляем представление JSON для [объекта userExperienceAnalyticsOverview.](../resources/intune-devices-userexperienceanalyticsoverview.md)</span><span class="sxs-lookup"><span data-stu-id="6765b-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>

<span data-ttu-id="6765b-129">В следующей таблице показаны свойства, необходимые при создании [userExperienceAnalyticsOverview.](../resources/intune-devices-userexperienceanalyticsoverview.md)</span><span class="sxs-lookup"><span data-stu-id="6765b-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md).</span></span>

|<span data-ttu-id="6765b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6765b-130">Property</span></span>|<span data-ttu-id="6765b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6765b-131">Type</span></span>|<span data-ttu-id="6765b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6765b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6765b-133">id</span><span class="sxs-lookup"><span data-stu-id="6765b-133">id</span></span>|<span data-ttu-id="6765b-134">String</span><span class="sxs-lookup"><span data-stu-id="6765b-134">String</span></span>|<span data-ttu-id="6765b-135">Уникальный идентификатор обзора аналитики пользовательских интерфейсов.</span><span class="sxs-lookup"><span data-stu-id="6765b-135">The unique identifier of the user experience analytics overview.</span></span>|
|<span data-ttu-id="6765b-136">overallScore</span><span class="sxs-lookup"><span data-stu-id="6765b-136">overallScore</span></span>|<span data-ttu-id="6765b-137">Int32</span><span class="sxs-lookup"><span data-stu-id="6765b-137">Int32</span></span>|<span data-ttu-id="6765b-138">Общая оценка аналитики пользовательского опыта.</span><span class="sxs-lookup"><span data-stu-id="6765b-138">The user experience analytics overall score.</span></span>|
|<span data-ttu-id="6765b-139">deviceBootPerformanceOverallScore</span><span class="sxs-lookup"><span data-stu-id="6765b-139">deviceBootPerformanceOverallScore</span></span>|<span data-ttu-id="6765b-140">Int32</span><span class="sxs-lookup"><span data-stu-id="6765b-140">Int32</span></span>|<span data-ttu-id="6765b-141">Общая оценка производительности загрузки устройства для аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="6765b-141">The user experience analytics device boot performance overall score.</span></span>|
|<span data-ttu-id="6765b-142">bestPracticesOverallScore</span><span class="sxs-lookup"><span data-stu-id="6765b-142">bestPracticesOverallScore</span></span>|<span data-ttu-id="6765b-143">Int32</span><span class="sxs-lookup"><span data-stu-id="6765b-143">Int32</span></span>|<span data-ttu-id="6765b-144">Анализ пользовательских интерфейсов позволяет опытом работы с общим показателем.</span><span class="sxs-lookup"><span data-stu-id="6765b-144">The user experience analytics best practices overall score.</span></span>|
|<span data-ttu-id="6765b-145">workFromAnywhereOverallScore</span><span class="sxs-lookup"><span data-stu-id="6765b-145">workFromAnywhereOverallScore</span></span>|<span data-ttu-id="6765b-146">Int32</span><span class="sxs-lookup"><span data-stu-id="6765b-146">Int32</span></span>|<span data-ttu-id="6765b-147">Аналитика пользовательского интерфейса Работает с любого общего балла.</span><span class="sxs-lookup"><span data-stu-id="6765b-147">The user experience analytics Work From Anywhere overall score.</span></span>|
|<span data-ttu-id="6765b-148">appHealthOverallScore</span><span class="sxs-lookup"><span data-stu-id="6765b-148">appHealthOverallScore</span></span>|<span data-ttu-id="6765b-149">Int32</span><span class="sxs-lookup"><span data-stu-id="6765b-149">Int32</span></span>|<span data-ttu-id="6765b-150">Общее состояние здоровья приложения для аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="6765b-150">The user experience analytics app health overall score.</span></span>|
|<span data-ttu-id="6765b-151">resourcePerformanceOverallScore</span><span class="sxs-lookup"><span data-stu-id="6765b-151">resourcePerformanceOverallScore</span></span>|<span data-ttu-id="6765b-152">Int32</span><span class="sxs-lookup"><span data-stu-id="6765b-152">Int32</span></span>|<span data-ttu-id="6765b-153">Общая оценка производительности ресурсов аналитики пользовательских ресурсов.</span><span class="sxs-lookup"><span data-stu-id="6765b-153">The user experience analytics resource performance overall score.</span></span>|
|<span data-ttu-id="6765b-154">insights</span><span class="sxs-lookup"><span data-stu-id="6765b-154">insights</span></span>|<span data-ttu-id="6765b-155">[коллекция userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md)</span><span class="sxs-lookup"><span data-stu-id="6765b-155">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="6765b-156">Аналитические сведения о пользовательском опыте.</span><span class="sxs-lookup"><span data-stu-id="6765b-156">The user experience analytics insights.</span></span>|
|<span data-ttu-id="6765b-157">state</span><span class="sxs-lookup"><span data-stu-id="6765b-157">state</span></span>|[<span data-ttu-id="6765b-158">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="6765b-158">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="6765b-159">Текущее состояние состояния состояния аналитики пользовательских интерфейсов.</span><span class="sxs-lookup"><span data-stu-id="6765b-159">The current health state of the user experience analytics overview.</span></span> <span data-ttu-id="6765b-160">Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="6765b-160">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="6765b-161">deviceBootPerformanceHealthState</span><span class="sxs-lookup"><span data-stu-id="6765b-161">deviceBootPerformanceHealthState</span></span>|[<span data-ttu-id="6765b-162">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="6765b-162">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="6765b-163">Текущее состояние состояния состояния аналитики пользовательского интерфейса категории BootPerformance.</span><span class="sxs-lookup"><span data-stu-id="6765b-163">The current health state of the user experience analytics 'BootPerformance' category.</span></span> <span data-ttu-id="6765b-164">Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="6765b-164">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="6765b-165">bestPracticesHealthState</span><span class="sxs-lookup"><span data-stu-id="6765b-165">bestPracticesHealthState</span></span>|[<span data-ttu-id="6765b-166">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="6765b-166">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="6765b-167">Текущее состояние здоровья категории аналитики пользовательских интерфейсов "BestPractices".</span><span class="sxs-lookup"><span data-stu-id="6765b-167">The current health state of the user experience analytics 'BestPractices' category.</span></span> <span data-ttu-id="6765b-168">Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="6765b-168">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="6765b-169">workFromAnywhereHealthState</span><span class="sxs-lookup"><span data-stu-id="6765b-169">workFromAnywhereHealthState</span></span>|[<span data-ttu-id="6765b-170">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="6765b-170">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="6765b-171">Текущее состояние состояния здоровья аналитики пользовательских интерфейсов категории WorkFromAnywhere.</span><span class="sxs-lookup"><span data-stu-id="6765b-171">The current health state of the user experience analytics 'WorkFromAnywhere' category.</span></span> <span data-ttu-id="6765b-172">Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="6765b-172">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="6765b-173">appHealthState</span><span class="sxs-lookup"><span data-stu-id="6765b-173">appHealthState</span></span>|[<span data-ttu-id="6765b-174">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="6765b-174">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="6765b-175">Текущее состояние здоровья категории аналитики пользовательских интерфейсов "BestPractices".</span><span class="sxs-lookup"><span data-stu-id="6765b-175">The current health state of the user experience analytics 'BestPractices' category.</span></span> <span data-ttu-id="6765b-176">Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="6765b-176">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="6765b-177">resourcePerformanceHealthState</span><span class="sxs-lookup"><span data-stu-id="6765b-177">resourcePerformanceHealthState</span></span>|[<span data-ttu-id="6765b-178">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="6765b-178">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="6765b-179">Текущее состояние состояния здоровья в категории аналитики пользовательского интерфейса "ResourcePerformance".</span><span class="sxs-lookup"><span data-stu-id="6765b-179">The current health state of the user experience analytics 'ResourcePerformance' category.</span></span> <span data-ttu-id="6765b-180">Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="6765b-180">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|



## <a name="response"></a><span data-ttu-id="6765b-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="6765b-181">Response</span></span>
<span data-ttu-id="6765b-182">В случае успеха этот метод возвращает код отклика и обновленный `200 OK` [объект userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="6765b-182">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6765b-183">Пример</span><span class="sxs-lookup"><span data-stu-id="6765b-183">Example</span></span>

### <a name="request"></a><span data-ttu-id="6765b-184">Запрос</span><span class="sxs-lookup"><span data-stu-id="6765b-184">Request</span></span>
<span data-ttu-id="6765b-185">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6765b-185">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsOverview
Content-type: application/json
Content-length: 1005

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
  "resourcePerformanceHealthState": "insufficientData"
}
```

### <a name="response"></a><span data-ttu-id="6765b-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="6765b-186">Response</span></span>
<span data-ttu-id="6765b-p108">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6765b-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1054

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
  "resourcePerformanceHealthState": "insufficientData"
}
```




