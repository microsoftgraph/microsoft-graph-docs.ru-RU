---
title: Обновление userExperienceAnalyticsOverview
description: Обновление свойств объекта userExperienceAnalyticsOverview.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 77d0107c7a1ca3255bcc87f60b3dba0ff140d133
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161238"
---
# <a name="update-userexperienceanalyticsoverview"></a><span data-ttu-id="43de7-103">Обновление userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="43de7-103">Update userExperienceAnalyticsOverview</span></span>

<span data-ttu-id="43de7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="43de7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="43de7-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43de7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="43de7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="43de7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43de7-107">Обновление свойств объекта [userExperienceAnalyticsOverview.](../resources/intune-devices-userexperienceanalyticsoverview.md)</span><span class="sxs-lookup"><span data-stu-id="43de7-107">Update the properties of a [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="43de7-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="43de7-108">Prerequisites</span></span>
<span data-ttu-id="43de7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43de7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43de7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="43de7-111">Permission type</span></span>|<span data-ttu-id="43de7-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="43de7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43de7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="43de7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="43de7-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43de7-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="43de7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="43de7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43de7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43de7-116">Not supported.</span></span>|
|<span data-ttu-id="43de7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="43de7-117">Application</span></span>|<span data-ttu-id="43de7-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43de7-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="43de7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="43de7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsOverview
```

## <a name="request-headers"></a><span data-ttu-id="43de7-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="43de7-120">Request headers</span></span>
|<span data-ttu-id="43de7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="43de7-121">Header</span></span>|<span data-ttu-id="43de7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="43de7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43de7-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="43de7-123">Authorization</span></span>|<span data-ttu-id="43de7-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="43de7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="43de7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="43de7-125">Accept</span></span>|<span data-ttu-id="43de7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="43de7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43de7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="43de7-127">Request body</span></span>
<span data-ttu-id="43de7-128">В теле запроса укажу представление объекта [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="43de7-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>

<span data-ttu-id="43de7-129">В следующей таблице показаны свойства, необходимые при создании [объекта userExperienceAnalyticsOverview.](../resources/intune-devices-userexperienceanalyticsoverview.md)</span><span class="sxs-lookup"><span data-stu-id="43de7-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md).</span></span>

|<span data-ttu-id="43de7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="43de7-130">Property</span></span>|<span data-ttu-id="43de7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="43de7-131">Type</span></span>|<span data-ttu-id="43de7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="43de7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43de7-133">id</span><span class="sxs-lookup"><span data-stu-id="43de7-133">id</span></span>|<span data-ttu-id="43de7-134">String</span><span class="sxs-lookup"><span data-stu-id="43de7-134">String</span></span>|<span data-ttu-id="43de7-135">Уникальный идентификатор обзора аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="43de7-135">The unique identifier of the user experience analytics overview.</span></span>|
|<span data-ttu-id="43de7-136">overallScore</span><span class="sxs-lookup"><span data-stu-id="43de7-136">overallScore</span></span>|<span data-ttu-id="43de7-137">Int32</span><span class="sxs-lookup"><span data-stu-id="43de7-137">Int32</span></span>|<span data-ttu-id="43de7-138">Общая оценка аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="43de7-138">The user experience analytics overall score.</span></span>|
|<span data-ttu-id="43de7-139">deviceBootPerformanceOverallScore</span><span class="sxs-lookup"><span data-stu-id="43de7-139">deviceBootPerformanceOverallScore</span></span>|<span data-ttu-id="43de7-140">Int32</span><span class="sxs-lookup"><span data-stu-id="43de7-140">Int32</span></span>|<span data-ttu-id="43de7-141">Общая производительность загрузки устройства аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="43de7-141">The user experience analytics device boot performance overall score.</span></span>|
|<span data-ttu-id="43de7-142">bestPracticesOverallScore</span><span class="sxs-lookup"><span data-stu-id="43de7-142">bestPracticesOverallScore</span></span>|<span data-ttu-id="43de7-143">Int32</span><span class="sxs-lookup"><span data-stu-id="43de7-143">Int32</span></span>|<span data-ttu-id="43de7-144">Общие методики анализа пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="43de7-144">The user experience analytics best practices overall score.</span></span>|
|<span data-ttu-id="43de7-145">appHealthOverallScore</span><span class="sxs-lookup"><span data-stu-id="43de7-145">appHealthOverallScore</span></span>|<span data-ttu-id="43de7-146">Int32</span><span class="sxs-lookup"><span data-stu-id="43de7-146">Int32</span></span>|<span data-ttu-id="43de7-147">Общая оценка состояния приложения аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="43de7-147">The user experience analytics app health overall score.</span></span>|
|<span data-ttu-id="43de7-148">insights</span><span class="sxs-lookup"><span data-stu-id="43de7-148">insights</span></span>|<span data-ttu-id="43de7-149">[Коллекция userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md)</span><span class="sxs-lookup"><span data-stu-id="43de7-149">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="43de7-150">Аналитика пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="43de7-150">The user experience analytics insights.</span></span>|
|<span data-ttu-id="43de7-151">state</span><span class="sxs-lookup"><span data-stu-id="43de7-151">state</span></span>|[<span data-ttu-id="43de7-152">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="43de7-152">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="43de7-153">Текущее состояние состояния анализа пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="43de7-153">The current health state of the user experience analytics overview.</span></span> <span data-ttu-id="43de7-154">Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="43de7-154">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="43de7-155">deviceBootPerformanceHealthState</span><span class="sxs-lookup"><span data-stu-id="43de7-155">deviceBootPerformanceHealthState</span></span>|[<span data-ttu-id="43de7-156">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="43de7-156">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="43de7-157">Текущее состояние состояния аналитики пользовательского интерфейса "BootPerformance".</span><span class="sxs-lookup"><span data-stu-id="43de7-157">The current health state of the user experience analytics 'BootPerformance' category.</span></span> <span data-ttu-id="43de7-158">Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="43de7-158">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="43de7-159">bestPracticesHealthState</span><span class="sxs-lookup"><span data-stu-id="43de7-159">bestPracticesHealthState</span></span>|[<span data-ttu-id="43de7-160">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="43de7-160">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="43de7-161">Текущее состояние состояния аналитики пользовательского интерфейса категории "BestPractices".</span><span class="sxs-lookup"><span data-stu-id="43de7-161">The current health state of the user experience analytics 'BestPractices' category.</span></span> <span data-ttu-id="43de7-162">Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="43de7-162">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="43de7-163">appHealthState</span><span class="sxs-lookup"><span data-stu-id="43de7-163">appHealthState</span></span>|[<span data-ttu-id="43de7-164">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="43de7-164">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="43de7-165">Текущее состояние состояния аналитики пользовательского интерфейса категории "BestPractices".</span><span class="sxs-lookup"><span data-stu-id="43de7-165">The current health state of the user experience analytics 'BestPractices' category.</span></span> <span data-ttu-id="43de7-166">Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="43de7-166">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|



## <a name="response"></a><span data-ttu-id="43de7-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="43de7-167">Response</span></span>
<span data-ttu-id="43de7-168">В случае успеха этот метод возвращает код отклика и обновленный объект `200 OK` [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="43de7-168">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43de7-169">Пример</span><span class="sxs-lookup"><span data-stu-id="43de7-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="43de7-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="43de7-170">Request</span></span>
<span data-ttu-id="43de7-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="43de7-171">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsOverview
Content-type: application/json
Content-length: 813

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsOverview",
  "overallScore": 12,
  "deviceBootPerformanceOverallScore": 1,
  "bestPracticesOverallScore": 9,
  "appHealthOverallScore": 5,
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
  "appHealthState": "insufficientData"
}
```

### <a name="response"></a><span data-ttu-id="43de7-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="43de7-172">Response</span></span>
<span data-ttu-id="43de7-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="43de7-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 862

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsOverview",
  "id": "8228da2b-da2b-8228-2bda-28822bda2882",
  "overallScore": 12,
  "deviceBootPerformanceOverallScore": 1,
  "bestPracticesOverallScore": 9,
  "appHealthOverallScore": 5,
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
  "appHealthState": "insufficientData"
}
```




