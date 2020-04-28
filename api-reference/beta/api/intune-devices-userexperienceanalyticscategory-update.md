---
title: Обновление Усерекспериенцеаналитикскатегори
description: Обновление свойств объекта Усерекспериенцеаналитикскатегори.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 550aea2dce1fb11c6888f8652ef39b9d0a6d84cb
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43322593"
---
# <a name="update-userexperienceanalyticscategory"></a><span data-ttu-id="53c15-103">Обновление Усерекспериенцеаналитикскатегори</span><span class="sxs-lookup"><span data-stu-id="53c15-103">Update userExperienceAnalyticsCategory</span></span>

<span data-ttu-id="53c15-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53c15-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="53c15-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53c15-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="53c15-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="53c15-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53c15-107">Обновление свойств объекта [усерекспериенцеаналитикскатегори](../resources/intune-devices-userexperienceanalyticscategory.md) .</span><span class="sxs-lookup"><span data-stu-id="53c15-107">Update the properties of a [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="53c15-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="53c15-108">Prerequisites</span></span>
<span data-ttu-id="53c15-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53c15-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53c15-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="53c15-111">Permission type</span></span>|<span data-ttu-id="53c15-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="53c15-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53c15-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="53c15-113">Delegated (work or school account)</span></span>|<span data-ttu-id="53c15-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53c15-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="53c15-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="53c15-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53c15-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53c15-116">Not supported.</span></span>|
|<span data-ttu-id="53c15-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="53c15-117">Application</span></span>|<span data-ttu-id="53c15-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53c15-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="53c15-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="53c15-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsCategories/{userExperienceAnalyticsCategoryId}
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/bestPracticesMetrics
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/deviceBootPerformanceMetrics
```

## <a name="request-headers"></a><span data-ttu-id="53c15-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="53c15-120">Request headers</span></span>
|<span data-ttu-id="53c15-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="53c15-121">Header</span></span>|<span data-ttu-id="53c15-122">Значение</span><span class="sxs-lookup"><span data-stu-id="53c15-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53c15-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="53c15-123">Authorization</span></span>|<span data-ttu-id="53c15-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="53c15-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53c15-125">Accept</span><span class="sxs-lookup"><span data-stu-id="53c15-125">Accept</span></span>|<span data-ttu-id="53c15-126">application/json</span><span class="sxs-lookup"><span data-stu-id="53c15-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53c15-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="53c15-127">Request body</span></span>
<span data-ttu-id="53c15-128">В тексте запроса добавьте представление объекта [усерекспериенцеаналитикскатегори](../resources/intune-devices-userexperienceanalyticscategory.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="53c15-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>

<span data-ttu-id="53c15-129">В следующей таблице приведены свойства, необходимые при создании [усерекспериенцеаналитикскатегори](../resources/intune-devices-userexperienceanalyticscategory.md).</span><span class="sxs-lookup"><span data-stu-id="53c15-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md).</span></span>

|<span data-ttu-id="53c15-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="53c15-130">Property</span></span>|<span data-ttu-id="53c15-131">Тип</span><span class="sxs-lookup"><span data-stu-id="53c15-131">Type</span></span>|<span data-ttu-id="53c15-132">Описание</span><span class="sxs-lookup"><span data-stu-id="53c15-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53c15-133">id</span><span class="sxs-lookup"><span data-stu-id="53c15-133">id</span></span>|<span data-ttu-id="53c15-134">String</span><span class="sxs-lookup"><span data-stu-id="53c15-134">String</span></span>|<span data-ttu-id="53c15-135">Уникальный идентификатор категории аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="53c15-135">The unique identifier of the user experience analytics category.</span></span>|
|<span data-ttu-id="53c15-136">овераллскоре</span><span class="sxs-lookup"><span data-stu-id="53c15-136">overallScore</span></span>|<span data-ttu-id="53c15-137">Int32</span><span class="sxs-lookup"><span data-stu-id="53c15-137">Int32</span></span>|<span data-ttu-id="53c15-138">Общий показатель категории аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="53c15-138">The overall score of the user experience analytics category.</span></span>|
|<span data-ttu-id="53c15-139">insights</span><span class="sxs-lookup"><span data-stu-id="53c15-139">insights</span></span>|<span data-ttu-id="53c15-140">Коллекция [усерекспериенцеаналитиксинсигхт](../resources/intune-devices-userexperienceanalyticsinsight.md)</span><span class="sxs-lookup"><span data-stu-id="53c15-140">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="53c15-141">Аналитика для категории аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="53c15-141">The insights for the user experience analytics category.</span></span>|
|<span data-ttu-id="53c15-142">state</span><span class="sxs-lookup"><span data-stu-id="53c15-142">state</span></span>|[<span data-ttu-id="53c15-143">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="53c15-143">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="53c15-144">Текущее состояние работоспособности категории аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="53c15-144">The current health state of the user experience analytics category.</span></span> <span data-ttu-id="53c15-145">Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="53c15-145">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|



## <a name="response"></a><span data-ttu-id="53c15-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="53c15-146">Response</span></span>
<span data-ttu-id="53c15-147">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [усерекспериенцеаналитикскатегори](../resources/intune-devices-userexperienceanalyticscategory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="53c15-147">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53c15-148">Пример</span><span class="sxs-lookup"><span data-stu-id="53c15-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="53c15-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="53c15-149">Request</span></span>
<span data-ttu-id="53c15-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="53c15-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="53c15-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="53c15-151">Response</span></span>
<span data-ttu-id="53c15-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="53c15-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



