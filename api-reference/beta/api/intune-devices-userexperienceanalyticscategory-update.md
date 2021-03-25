---
title: Обновление userExperienceAnalyticsCategory
description: Обновление свойств объекта userExperienceAnalyticsCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 23f89e530972e3510efc8051d065c28a5cef7c89
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51154240"
---
# <a name="update-userexperienceanalyticscategory"></a><span data-ttu-id="becca-103">Обновление userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="becca-103">Update userExperienceAnalyticsCategory</span></span>

<span data-ttu-id="becca-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="becca-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="becca-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="becca-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="becca-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="becca-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="becca-107">Обновление свойств объекта [userExperienceAnalyticsCategory.](../resources/intune-devices-userexperienceanalyticscategory.md)</span><span class="sxs-lookup"><span data-stu-id="becca-107">Update the properties of a [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="becca-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="becca-108">Prerequisites</span></span>
<span data-ttu-id="becca-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="becca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="becca-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="becca-111">Permission type</span></span>|<span data-ttu-id="becca-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="becca-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="becca-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="becca-113">Delegated (work or school account)</span></span>|<span data-ttu-id="becca-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="becca-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="becca-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="becca-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="becca-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="becca-116">Not supported.</span></span>|
|<span data-ttu-id="becca-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="becca-117">Application</span></span>|<span data-ttu-id="becca-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="becca-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="becca-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="becca-119">HTTP Request</span></span>
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
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/workFromAnywhereMetrics
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/resourcePerformanceMetrics
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/deviceBootPerformanceMetrics
```

## <a name="request-headers"></a><span data-ttu-id="becca-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="becca-120">Request headers</span></span>
|<span data-ttu-id="becca-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="becca-121">Header</span></span>|<span data-ttu-id="becca-122">Значение</span><span class="sxs-lookup"><span data-stu-id="becca-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="becca-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="becca-123">Authorization</span></span>|<span data-ttu-id="becca-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="becca-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="becca-125">Accept</span><span class="sxs-lookup"><span data-stu-id="becca-125">Accept</span></span>|<span data-ttu-id="becca-126">application/json</span><span class="sxs-lookup"><span data-stu-id="becca-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="becca-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="becca-127">Request body</span></span>
<span data-ttu-id="becca-128">В теле запроса поставляем представление JSON для [объекта userExperienceAnalyticsCategory.](../resources/intune-devices-userexperienceanalyticscategory.md)</span><span class="sxs-lookup"><span data-stu-id="becca-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>

<span data-ttu-id="becca-129">В следующей таблице показаны свойства, необходимые при создании [userExperienceAnalyticsCategory.](../resources/intune-devices-userexperienceanalyticscategory.md)</span><span class="sxs-lookup"><span data-stu-id="becca-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md).</span></span>

|<span data-ttu-id="becca-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="becca-130">Property</span></span>|<span data-ttu-id="becca-131">Тип</span><span class="sxs-lookup"><span data-stu-id="becca-131">Type</span></span>|<span data-ttu-id="becca-132">Описание</span><span class="sxs-lookup"><span data-stu-id="becca-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="becca-133">id</span><span class="sxs-lookup"><span data-stu-id="becca-133">id</span></span>|<span data-ttu-id="becca-134">Строка</span><span class="sxs-lookup"><span data-stu-id="becca-134">String</span></span>|<span data-ttu-id="becca-135">Уникальный идентификатор категории аналитики пользовательских интерфейсов.</span><span class="sxs-lookup"><span data-stu-id="becca-135">The unique identifier of the user experience analytics category.</span></span>|
|<span data-ttu-id="becca-136">overallScore</span><span class="sxs-lookup"><span data-stu-id="becca-136">overallScore</span></span>|<span data-ttu-id="becca-137">Int32</span><span class="sxs-lookup"><span data-stu-id="becca-137">Int32</span></span>|<span data-ttu-id="becca-138">Общая оценка категории аналитики пользовательских интерфейсов.</span><span class="sxs-lookup"><span data-stu-id="becca-138">The overall score of the user experience analytics category.</span></span>|
|<span data-ttu-id="becca-139">totalDevices</span><span class="sxs-lookup"><span data-stu-id="becca-139">totalDevices</span></span>|<span data-ttu-id="becca-140">Int32</span><span class="sxs-lookup"><span data-stu-id="becca-140">Int32</span></span>|<span data-ttu-id="becca-141">Общее число устройств категории аналитики пользовательских интерфейсов.</span><span class="sxs-lookup"><span data-stu-id="becca-141">The total device count of the user experience analytics category.</span></span>|
|<span data-ttu-id="becca-142">insights</span><span class="sxs-lookup"><span data-stu-id="becca-142">insights</span></span>|<span data-ttu-id="becca-143">[коллекция userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md)</span><span class="sxs-lookup"><span data-stu-id="becca-143">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="becca-144">Сведения о категории аналитики пользовательских интерфейсов.</span><span class="sxs-lookup"><span data-stu-id="becca-144">The insights for the user experience analytics category.</span></span>|
|<span data-ttu-id="becca-145">state</span><span class="sxs-lookup"><span data-stu-id="becca-145">state</span></span>|[<span data-ttu-id="becca-146">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="becca-146">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="becca-147">Текущее состояние здоровья категории аналитики пользовательских интерфейсов.</span><span class="sxs-lookup"><span data-stu-id="becca-147">The current health state of the user experience analytics category.</span></span> <span data-ttu-id="becca-148">Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="becca-148">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|



## <a name="response"></a><span data-ttu-id="becca-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="becca-149">Response</span></span>
<span data-ttu-id="becca-150">В случае успешной работы этот метод возвращает код отклика и обновленный `200 OK` [объект userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="becca-150">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="becca-151">Пример</span><span class="sxs-lookup"><span data-stu-id="becca-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="becca-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="becca-152">Request</span></span>
<span data-ttu-id="becca-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="becca-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthOverview
Content-type: application/json
Content-length: 576

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsCategory",
  "overallScore": 12,
  "totalDevices": 12,
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

### <a name="response"></a><span data-ttu-id="becca-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="becca-154">Response</span></span>
<span data-ttu-id="becca-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="becca-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 625

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsCategory",
  "id": "cfd28056-8056-cfd2-5680-d2cf5680d2cf",
  "overallScore": 12,
  "totalDevices": 12,
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




