---
title: Обновление Усерекспериенцеаналитикскатегори
description: Обновление свойств объекта Усерекспериенцеаналитикскатегори.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e011518074dd7fe0588ab850fda1a65ac1c01ce5
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42814002"
---
# <a name="update-userexperienceanalyticscategory"></a><span data-ttu-id="945cf-103">Обновление Усерекспериенцеаналитикскатегори</span><span class="sxs-lookup"><span data-stu-id="945cf-103">Update userExperienceAnalyticsCategory</span></span>

> <span data-ttu-id="945cf-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="945cf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="945cf-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="945cf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="945cf-106">Обновление свойств объекта [усерекспериенцеаналитикскатегори](../resources/intune-devices-userexperienceanalyticscategory.md) .</span><span class="sxs-lookup"><span data-stu-id="945cf-106">Update the properties of a [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="945cf-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="945cf-107">Prerequisites</span></span>
<span data-ttu-id="945cf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="945cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="945cf-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="945cf-110">Permission type</span></span>|<span data-ttu-id="945cf-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="945cf-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="945cf-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="945cf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="945cf-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="945cf-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="945cf-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="945cf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="945cf-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="945cf-115">Not supported.</span></span>|
|<span data-ttu-id="945cf-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="945cf-116">Application</span></span>|<span data-ttu-id="945cf-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="945cf-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="945cf-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="945cf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsCategories/{userExperienceAnalyticsCategoryId}
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/bestPracticesMetrics
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/deviceBootPerformanceMetrics
```

## <a name="request-headers"></a><span data-ttu-id="945cf-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="945cf-119">Request headers</span></span>
|<span data-ttu-id="945cf-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="945cf-120">Header</span></span>|<span data-ttu-id="945cf-121">Значение</span><span class="sxs-lookup"><span data-stu-id="945cf-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="945cf-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="945cf-122">Authorization</span></span>|<span data-ttu-id="945cf-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="945cf-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="945cf-124">Accept</span><span class="sxs-lookup"><span data-stu-id="945cf-124">Accept</span></span>|<span data-ttu-id="945cf-125">application/json</span><span class="sxs-lookup"><span data-stu-id="945cf-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="945cf-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="945cf-126">Request body</span></span>
<span data-ttu-id="945cf-127">В тексте запроса добавьте представление объекта [усерекспериенцеаналитикскатегори](../resources/intune-devices-userexperienceanalyticscategory.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="945cf-127">In the request body, supply a JSON representation for the [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>

<span data-ttu-id="945cf-128">В следующей таблице приведены свойства, необходимые при создании [усерекспериенцеаналитикскатегори](../resources/intune-devices-userexperienceanalyticscategory.md).</span><span class="sxs-lookup"><span data-stu-id="945cf-128">The following table shows the properties that are required when you create the [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md).</span></span>

|<span data-ttu-id="945cf-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="945cf-129">Property</span></span>|<span data-ttu-id="945cf-130">Тип</span><span class="sxs-lookup"><span data-stu-id="945cf-130">Type</span></span>|<span data-ttu-id="945cf-131">Описание</span><span class="sxs-lookup"><span data-stu-id="945cf-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="945cf-132">id</span><span class="sxs-lookup"><span data-stu-id="945cf-132">id</span></span>|<span data-ttu-id="945cf-133">String</span><span class="sxs-lookup"><span data-stu-id="945cf-133">String</span></span>|<span data-ttu-id="945cf-134">Уникальный идентификатор категории аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="945cf-134">The unique identifier of the user experience analytics category.</span></span>|
|<span data-ttu-id="945cf-135">овераллскоре</span><span class="sxs-lookup"><span data-stu-id="945cf-135">overallScore</span></span>|<span data-ttu-id="945cf-136">Int32</span><span class="sxs-lookup"><span data-stu-id="945cf-136">Int32</span></span>|<span data-ttu-id="945cf-137">Общий показатель категории аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="945cf-137">The overall score of the user experience analytics category.</span></span>|
|<span data-ttu-id="945cf-138">insights</span><span class="sxs-lookup"><span data-stu-id="945cf-138">insights</span></span>|<span data-ttu-id="945cf-139">Коллекция [усерекспериенцеаналитиксинсигхт](../resources/intune-devices-userexperienceanalyticsinsight.md)</span><span class="sxs-lookup"><span data-stu-id="945cf-139">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="945cf-140">Аналитика для категории аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="945cf-140">The insights for the user experience analytics category.</span></span>|
|<span data-ttu-id="945cf-141">state</span><span class="sxs-lookup"><span data-stu-id="945cf-141">state</span></span>|[<span data-ttu-id="945cf-142">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="945cf-142">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="945cf-143">Текущее состояние работоспособности категории аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="945cf-143">The current health state of the user experience analytics category.</span></span> <span data-ttu-id="945cf-144">Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="945cf-144">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|



## <a name="response"></a><span data-ttu-id="945cf-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="945cf-145">Response</span></span>
<span data-ttu-id="945cf-146">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [усерекспериенцеаналитикскатегори](../resources/intune-devices-userexperienceanalyticscategory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="945cf-146">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="945cf-147">Пример</span><span class="sxs-lookup"><span data-stu-id="945cf-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="945cf-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="945cf-148">Request</span></span>
<span data-ttu-id="945cf-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="945cf-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsCategories/{userExperienceAnalyticsCategoryId}
Content-type: application/json
Content-length: 572

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
          "value": "<Unknown Primitive Type Edm.Double>"
        }
      ],
      "severity": "informational"
    }
  ],
  "state": "insufficientData"
}
```

### <a name="response"></a><span data-ttu-id="945cf-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="945cf-150">Response</span></span>
<span data-ttu-id="945cf-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="945cf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 621

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
          "value": "<Unknown Primitive Type Edm.Double>"
        }
      ],
      "severity": "informational"
    }
  ],
  "state": "insufficientData"
}
```




