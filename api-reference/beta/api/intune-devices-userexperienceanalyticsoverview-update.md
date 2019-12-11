---
title: Обновление Усерекспериенцеаналитиксовервиев
description: Обновление свойств объекта Усерекспериенцеаналитиксовервиев.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e2140a8955b49f0f792058dffd6c743d75b8bd97
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39944395"
---
# <a name="update-userexperienceanalyticsoverview"></a><span data-ttu-id="481c7-103">Обновление Усерекспериенцеаналитиксовервиев</span><span class="sxs-lookup"><span data-stu-id="481c7-103">Update userExperienceAnalyticsOverview</span></span>

> <span data-ttu-id="481c7-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="481c7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="481c7-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="481c7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="481c7-106">Обновление свойств объекта [усерекспериенцеаналитиксовервиев](../resources/intune-devices-userexperienceanalyticsoverview.md) .</span><span class="sxs-lookup"><span data-stu-id="481c7-106">Update the properties of a [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="481c7-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="481c7-107">Prerequisites</span></span>
<span data-ttu-id="481c7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="481c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="481c7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="481c7-110">Permission type</span></span>|<span data-ttu-id="481c7-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="481c7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="481c7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="481c7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="481c7-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="481c7-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="481c7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="481c7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="481c7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="481c7-115">Not supported.</span></span>|
|<span data-ttu-id="481c7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="481c7-116">Application</span></span>|<span data-ttu-id="481c7-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="481c7-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="481c7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="481c7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsOverview
```

## <a name="request-headers"></a><span data-ttu-id="481c7-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="481c7-119">Request headers</span></span>
|<span data-ttu-id="481c7-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="481c7-120">Header</span></span>|<span data-ttu-id="481c7-121">Значение</span><span class="sxs-lookup"><span data-stu-id="481c7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="481c7-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="481c7-122">Authorization</span></span>|<span data-ttu-id="481c7-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="481c7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="481c7-124">Accept</span><span class="sxs-lookup"><span data-stu-id="481c7-124">Accept</span></span>|<span data-ttu-id="481c7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="481c7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="481c7-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="481c7-126">Request body</span></span>
<span data-ttu-id="481c7-127">В тексте запроса добавьте представление объекта [усерекспериенцеаналитиксовервиев](../resources/intune-devices-userexperienceanalyticsoverview.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="481c7-127">In the request body, supply a JSON representation for the [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>

<span data-ttu-id="481c7-128">В следующей таблице приведены свойства, необходимые при создании [усерекспериенцеаналитиксовервиев](../resources/intune-devices-userexperienceanalyticsoverview.md).</span><span class="sxs-lookup"><span data-stu-id="481c7-128">The following table shows the properties that are required when you create the [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md).</span></span>

|<span data-ttu-id="481c7-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="481c7-129">Property</span></span>|<span data-ttu-id="481c7-130">Тип</span><span class="sxs-lookup"><span data-stu-id="481c7-130">Type</span></span>|<span data-ttu-id="481c7-131">Описание</span><span class="sxs-lookup"><span data-stu-id="481c7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="481c7-132">id</span><span class="sxs-lookup"><span data-stu-id="481c7-132">id</span></span>|<span data-ttu-id="481c7-133">Строка</span><span class="sxs-lookup"><span data-stu-id="481c7-133">String</span></span>|<span data-ttu-id="481c7-134">Уникальный идентификатор для обзора аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="481c7-134">The unique identifier of the user experience analytics overview.</span></span>|
|<span data-ttu-id="481c7-135">овераллскоре</span><span class="sxs-lookup"><span data-stu-id="481c7-135">overallScore</span></span>|<span data-ttu-id="481c7-136">Int32</span><span class="sxs-lookup"><span data-stu-id="481c7-136">Int32</span></span>|<span data-ttu-id="481c7-137">Общий показатель аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="481c7-137">The user experience analytics overall score.</span></span>|
|<span data-ttu-id="481c7-138">девицебутперформанцеовераллскоре</span><span class="sxs-lookup"><span data-stu-id="481c7-138">deviceBootPerformanceOverallScore</span></span>|<span data-ttu-id="481c7-139">Int32</span><span class="sxs-lookup"><span data-stu-id="481c7-139">Int32</span></span>|<span data-ttu-id="481c7-140">Общая оценка производительности при загрузке устройства Analytics.</span><span class="sxs-lookup"><span data-stu-id="481c7-140">The user experience analytics device boot performance overall score.</span></span>|
|<span data-ttu-id="481c7-141">бестпрактицесовераллскоре</span><span class="sxs-lookup"><span data-stu-id="481c7-141">bestPracticesOverallScore</span></span>|<span data-ttu-id="481c7-142">Int32</span><span class="sxs-lookup"><span data-stu-id="481c7-142">Int32</span></span>|<span data-ttu-id="481c7-143">Общая оценка рекомендаций по анализу пользовательских интерфейсов.</span><span class="sxs-lookup"><span data-stu-id="481c7-143">The user experience analytics best practices overall score.</span></span>|
|<span data-ttu-id="481c7-144">insights</span><span class="sxs-lookup"><span data-stu-id="481c7-144">insights</span></span>|<span data-ttu-id="481c7-145">Коллекция [усерекспериенцеаналитиксинсигхт](../resources/intune-devices-userexperienceanalyticsinsight.md)</span><span class="sxs-lookup"><span data-stu-id="481c7-145">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="481c7-146">Аналитика взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="481c7-146">The user experience analytics insights.</span></span>|
|<span data-ttu-id="481c7-147">state</span><span class="sxs-lookup"><span data-stu-id="481c7-147">state</span></span>|[<span data-ttu-id="481c7-148">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="481c7-148">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="481c7-149">Текущее состояние работоспособности в обзоре аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="481c7-149">The current health state of the user experience analytics overview.</span></span> <span data-ttu-id="481c7-150">Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="481c7-150">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="481c7-151">девицебутперформанцехеалсстате</span><span class="sxs-lookup"><span data-stu-id="481c7-151">deviceBootPerformanceHealthState</span></span>|[<span data-ttu-id="481c7-152">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="481c7-152">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="481c7-153">Текущее состояние работоспособности категории аналитики взаимодействия с пользователем "Бутперформанце".</span><span class="sxs-lookup"><span data-stu-id="481c7-153">The current health state of the user experience analytics 'BootPerformance' category.</span></span> <span data-ttu-id="481c7-154">Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="481c7-154">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="481c7-155">бестпрактицешеалсстате</span><span class="sxs-lookup"><span data-stu-id="481c7-155">bestPracticesHealthState</span></span>|[<span data-ttu-id="481c7-156">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="481c7-156">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="481c7-157">Текущее состояние работоспособности категории аналитики взаимодействия с пользователем "Бестпрактицес".</span><span class="sxs-lookup"><span data-stu-id="481c7-157">The current health state of the user experience analytics 'BestPractices' category.</span></span> <span data-ttu-id="481c7-158">Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="481c7-158">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|



## <a name="response"></a><span data-ttu-id="481c7-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="481c7-159">Response</span></span>
<span data-ttu-id="481c7-160">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [усерекспериенцеаналитиксовервиев](../resources/intune-devices-userexperienceanalyticsoverview.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="481c7-160">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="481c7-161">Пример</span><span class="sxs-lookup"><span data-stu-id="481c7-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="481c7-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="481c7-162">Request</span></span>
<span data-ttu-id="481c7-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="481c7-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="481c7-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="481c7-164">Response</span></span>
<span data-ttu-id="481c7-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="481c7-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





