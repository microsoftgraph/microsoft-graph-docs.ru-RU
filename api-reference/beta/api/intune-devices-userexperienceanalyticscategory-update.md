---
title: Обновление Усерекспериенцеаналитикскатегори
description: Обновление свойств объекта Усерекспериенцеаналитикскатегори.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d7309621128d2adfd41cdc7869bcfaea995ba500
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42468462"
---
# <a name="update-userexperienceanalyticscategory"></a><span data-ttu-id="d98a6-103">Обновление Усерекспериенцеаналитикскатегори</span><span class="sxs-lookup"><span data-stu-id="d98a6-103">Update userExperienceAnalyticsCategory</span></span>

<span data-ttu-id="d98a6-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d98a6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d98a6-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d98a6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d98a6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d98a6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d98a6-107">Обновление свойств объекта [усерекспериенцеаналитикскатегори](../resources/intune-devices-userexperienceanalyticscategory.md) .</span><span class="sxs-lookup"><span data-stu-id="d98a6-107">Update the properties of a [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d98a6-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d98a6-108">Prerequisites</span></span>
<span data-ttu-id="d98a6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d98a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d98a6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d98a6-111">Permission type</span></span>|<span data-ttu-id="d98a6-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d98a6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d98a6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d98a6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d98a6-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d98a6-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d98a6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d98a6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d98a6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d98a6-116">Not supported.</span></span>|
|<span data-ttu-id="d98a6-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d98a6-117">Application</span></span>|<span data-ttu-id="d98a6-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d98a6-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d98a6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d98a6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsCategories/{userExperienceAnalyticsCategoryId}
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/bestPracticesMetrics
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/deviceBootPerformanceMetrics
```

## <a name="request-headers"></a><span data-ttu-id="d98a6-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d98a6-120">Request headers</span></span>
|<span data-ttu-id="d98a6-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d98a6-121">Header</span></span>|<span data-ttu-id="d98a6-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d98a6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d98a6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d98a6-123">Authorization</span></span>|<span data-ttu-id="d98a6-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d98a6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d98a6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d98a6-125">Accept</span></span>|<span data-ttu-id="d98a6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d98a6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d98a6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d98a6-127">Request body</span></span>
<span data-ttu-id="d98a6-128">В тексте запроса добавьте представление объекта [усерекспериенцеаналитикскатегори](../resources/intune-devices-userexperienceanalyticscategory.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d98a6-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>

<span data-ttu-id="d98a6-129">В следующей таблице приведены свойства, необходимые при создании [усерекспериенцеаналитикскатегори](../resources/intune-devices-userexperienceanalyticscategory.md).</span><span class="sxs-lookup"><span data-stu-id="d98a6-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md).</span></span>

|<span data-ttu-id="d98a6-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d98a6-130">Property</span></span>|<span data-ttu-id="d98a6-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d98a6-131">Type</span></span>|<span data-ttu-id="d98a6-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d98a6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d98a6-133">id</span><span class="sxs-lookup"><span data-stu-id="d98a6-133">id</span></span>|<span data-ttu-id="d98a6-134">String</span><span class="sxs-lookup"><span data-stu-id="d98a6-134">String</span></span>|<span data-ttu-id="d98a6-135">Уникальный идентификатор категории аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="d98a6-135">The unique identifier of the user experience analytics category.</span></span>|
|<span data-ttu-id="d98a6-136">овераллскоре</span><span class="sxs-lookup"><span data-stu-id="d98a6-136">overallScore</span></span>|<span data-ttu-id="d98a6-137">Int32</span><span class="sxs-lookup"><span data-stu-id="d98a6-137">Int32</span></span>|<span data-ttu-id="d98a6-138">Общий показатель категории аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="d98a6-138">The overall score of the user experience analytics category.</span></span>|
|<span data-ttu-id="d98a6-139">insights</span><span class="sxs-lookup"><span data-stu-id="d98a6-139">insights</span></span>|<span data-ttu-id="d98a6-140">Коллекция [усерекспериенцеаналитиксинсигхт](../resources/intune-devices-userexperienceanalyticsinsight.md)</span><span class="sxs-lookup"><span data-stu-id="d98a6-140">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="d98a6-141">Аналитика для категории аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="d98a6-141">The insights for the user experience analytics category.</span></span>|
|<span data-ttu-id="d98a6-142">state</span><span class="sxs-lookup"><span data-stu-id="d98a6-142">state</span></span>|[<span data-ttu-id="d98a6-143">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="d98a6-143">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="d98a6-144">Текущее состояние работоспособности категории аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="d98a6-144">The current health state of the user experience analytics category.</span></span> <span data-ttu-id="d98a6-145">Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="d98a6-145">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|



## <a name="response"></a><span data-ttu-id="d98a6-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="d98a6-146">Response</span></span>
<span data-ttu-id="d98a6-147">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [усерекспериенцеаналитикскатегори](../resources/intune-devices-userexperienceanalyticscategory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d98a6-147">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d98a6-148">Пример</span><span class="sxs-lookup"><span data-stu-id="d98a6-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="d98a6-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="d98a6-149">Request</span></span>
<span data-ttu-id="d98a6-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d98a6-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d98a6-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="d98a6-151">Response</span></span>
<span data-ttu-id="d98a6-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d98a6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





