---
title: Обновление Усерекспериенцеаналитиксовервиев
description: Обновление свойств объекта Усерекспериенцеаналитиксовервиев.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3ab0d189772159ceec940d4434611621cff7bcfb
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43379140"
---
# <a name="update-userexperienceanalyticsoverview"></a><span data-ttu-id="fe33d-103">Обновление Усерекспериенцеаналитиксовервиев</span><span class="sxs-lookup"><span data-stu-id="fe33d-103">Update userExperienceAnalyticsOverview</span></span>

<span data-ttu-id="fe33d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe33d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fe33d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe33d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fe33d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fe33d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe33d-107">Обновление свойств объекта [усерекспериенцеаналитиксовервиев](../resources/intune-devices-userexperienceanalyticsoverview.md) .</span><span class="sxs-lookup"><span data-stu-id="fe33d-107">Update the properties of a [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fe33d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fe33d-108">Prerequisites</span></span>
<span data-ttu-id="fe33d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe33d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe33d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fe33d-111">Permission type</span></span>|<span data-ttu-id="fe33d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fe33d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fe33d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fe33d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fe33d-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe33d-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="fe33d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fe33d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fe33d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe33d-116">Not supported.</span></span>|
|<span data-ttu-id="fe33d-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="fe33d-117">Application</span></span>|<span data-ttu-id="fe33d-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe33d-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fe33d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fe33d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsOverview
```

## <a name="request-headers"></a><span data-ttu-id="fe33d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="fe33d-120">Request headers</span></span>
|<span data-ttu-id="fe33d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fe33d-121">Header</span></span>|<span data-ttu-id="fe33d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fe33d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fe33d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe33d-123">Authorization</span></span>|<span data-ttu-id="fe33d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fe33d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fe33d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fe33d-125">Accept</span></span>|<span data-ttu-id="fe33d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fe33d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe33d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fe33d-127">Request body</span></span>
<span data-ttu-id="fe33d-128">В тексте запроса добавьте представление объекта [усерекспериенцеаналитиксовервиев](../resources/intune-devices-userexperienceanalyticsoverview.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fe33d-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>

<span data-ttu-id="fe33d-129">В следующей таблице приведены свойства, необходимые при создании [усерекспериенцеаналитиксовервиев](../resources/intune-devices-userexperienceanalyticsoverview.md).</span><span class="sxs-lookup"><span data-stu-id="fe33d-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md).</span></span>

|<span data-ttu-id="fe33d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="fe33d-130">Property</span></span>|<span data-ttu-id="fe33d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="fe33d-131">Type</span></span>|<span data-ttu-id="fe33d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="fe33d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe33d-133">id</span><span class="sxs-lookup"><span data-stu-id="fe33d-133">id</span></span>|<span data-ttu-id="fe33d-134">String</span><span class="sxs-lookup"><span data-stu-id="fe33d-134">String</span></span>|<span data-ttu-id="fe33d-135">Уникальный идентификатор для обзора аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="fe33d-135">The unique identifier of the user experience analytics overview.</span></span>|
|<span data-ttu-id="fe33d-136">овераллскоре</span><span class="sxs-lookup"><span data-stu-id="fe33d-136">overallScore</span></span>|<span data-ttu-id="fe33d-137">Int32</span><span class="sxs-lookup"><span data-stu-id="fe33d-137">Int32</span></span>|<span data-ttu-id="fe33d-138">Общий показатель аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="fe33d-138">The user experience analytics overall score.</span></span>|
|<span data-ttu-id="fe33d-139">девицебутперформанцеовераллскоре</span><span class="sxs-lookup"><span data-stu-id="fe33d-139">deviceBootPerformanceOverallScore</span></span>|<span data-ttu-id="fe33d-140">Int32</span><span class="sxs-lookup"><span data-stu-id="fe33d-140">Int32</span></span>|<span data-ttu-id="fe33d-141">Общая оценка производительности при загрузке устройства Analytics.</span><span class="sxs-lookup"><span data-stu-id="fe33d-141">The user experience analytics device boot performance overall score.</span></span>|
|<span data-ttu-id="fe33d-142">бестпрактицесовераллскоре</span><span class="sxs-lookup"><span data-stu-id="fe33d-142">bestPracticesOverallScore</span></span>|<span data-ttu-id="fe33d-143">Int32</span><span class="sxs-lookup"><span data-stu-id="fe33d-143">Int32</span></span>|<span data-ttu-id="fe33d-144">Общая оценка рекомендаций по анализу пользовательских интерфейсов.</span><span class="sxs-lookup"><span data-stu-id="fe33d-144">The user experience analytics best practices overall score.</span></span>|
|<span data-ttu-id="fe33d-145">insights</span><span class="sxs-lookup"><span data-stu-id="fe33d-145">insights</span></span>|<span data-ttu-id="fe33d-146">Коллекция [усерекспериенцеаналитиксинсигхт](../resources/intune-devices-userexperienceanalyticsinsight.md)</span><span class="sxs-lookup"><span data-stu-id="fe33d-146">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="fe33d-147">Аналитика взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="fe33d-147">The user experience analytics insights.</span></span>|
|<span data-ttu-id="fe33d-148">state</span><span class="sxs-lookup"><span data-stu-id="fe33d-148">state</span></span>|[<span data-ttu-id="fe33d-149">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="fe33d-149">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="fe33d-150">Текущее состояние работоспособности в обзоре аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="fe33d-150">The current health state of the user experience analytics overview.</span></span> <span data-ttu-id="fe33d-151">Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="fe33d-151">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="fe33d-152">девицебутперформанцехеалсстате</span><span class="sxs-lookup"><span data-stu-id="fe33d-152">deviceBootPerformanceHealthState</span></span>|[<span data-ttu-id="fe33d-153">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="fe33d-153">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="fe33d-154">Текущее состояние работоспособности категории аналитики взаимодействия с пользователем "Бутперформанце".</span><span class="sxs-lookup"><span data-stu-id="fe33d-154">The current health state of the user experience analytics 'BootPerformance' category.</span></span> <span data-ttu-id="fe33d-155">Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="fe33d-155">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="fe33d-156">бестпрактицешеалсстате</span><span class="sxs-lookup"><span data-stu-id="fe33d-156">bestPracticesHealthState</span></span>|[<span data-ttu-id="fe33d-157">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="fe33d-157">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="fe33d-158">Текущее состояние работоспособности категории аналитики взаимодействия с пользователем "Бестпрактицес".</span><span class="sxs-lookup"><span data-stu-id="fe33d-158">The current health state of the user experience analytics 'BestPractices' category.</span></span> <span data-ttu-id="fe33d-159">Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="fe33d-159">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|



## <a name="response"></a><span data-ttu-id="fe33d-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="fe33d-160">Response</span></span>
<span data-ttu-id="fe33d-161">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [усерекспериенцеаналитиксовервиев](../resources/intune-devices-userexperienceanalyticsoverview.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fe33d-161">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe33d-162">Пример</span><span class="sxs-lookup"><span data-stu-id="fe33d-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="fe33d-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="fe33d-163">Request</span></span>
<span data-ttu-id="fe33d-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fe33d-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsOverview
Content-type: application/json
Content-length: 760

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsOverview",
  "overallScore": 12,
  "deviceBootPerformanceOverallScore": 1,
  "bestPracticesOverallScore": 9,
  "insights": [
    {
      "@odata.type": "microsoft.graph.userExperienceAnalyticsInsight",
      "userExperienceAnalyticsMetricId": "User Experience Analytics Metric Id value",
      "insightId": "Insight Id value",
      "values": [
        {
          "@odata.type": "microsoft.graph.insightValueDouble",
          "value": "<Unknown Primitive Type Edm.Double>"
        }
      ],
      "severity": "informational"
    }
  ],
  "state": "insufficientData",
  "deviceBootPerformanceHealthState": "insufficientData",
  "bestPracticesHealthState": "insufficientData"
}
```

### <a name="response"></a><span data-ttu-id="fe33d-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="fe33d-165">Response</span></span>
<span data-ttu-id="fe33d-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fe33d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 809

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsOverview",
  "id": "8228da2b-da2b-8228-2bda-28822bda2882",
  "overallScore": 12,
  "deviceBootPerformanceOverallScore": 1,
  "bestPracticesOverallScore": 9,
  "insights": [
    {
      "@odata.type": "microsoft.graph.userExperienceAnalyticsInsight",
      "userExperienceAnalyticsMetricId": "User Experience Analytics Metric Id value",
      "insightId": "Insight Id value",
      "values": [
        {
          "@odata.type": "microsoft.graph.insightValueDouble",
          "value": "<Unknown Primitive Type Edm.Double>"
        }
      ],
      "severity": "informational"
    }
  ],
  "state": "insufficientData",
  "deviceBootPerformanceHealthState": "insufficientData",
  "bestPracticesHealthState": "insufficientData"
}
```



