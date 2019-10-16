---
title: Обновление Усерекспериенцеаналитикскатегори
description: Обновление свойств объекта Усерекспериенцеаналитикскатегори.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7effcd00609850800533fe3b709a25842fa541e9
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37527389"
---
# <a name="update-userexperienceanalyticscategory"></a><span data-ttu-id="c19b6-103">Обновление Усерекспериенцеаналитикскатегори</span><span class="sxs-lookup"><span data-stu-id="c19b6-103">Update userExperienceAnalyticsCategory</span></span>

> <span data-ttu-id="c19b6-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c19b6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c19b6-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c19b6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c19b6-106">Обновление свойств объекта [усерекспериенцеаналитикскатегори](../resources/intune-devices-userexperienceanalyticscategory.md) .</span><span class="sxs-lookup"><span data-stu-id="c19b6-106">Update the properties of a [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c19b6-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c19b6-107">Prerequisites</span></span>
<span data-ttu-id="c19b6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c19b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c19b6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c19b6-110">Permission type</span></span>|<span data-ttu-id="c19b6-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c19b6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c19b6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c19b6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c19b6-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c19b6-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c19b6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c19b6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c19b6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c19b6-115">Not supported.</span></span>|
|<span data-ttu-id="c19b6-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="c19b6-116">Application</span></span>|<span data-ttu-id="c19b6-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c19b6-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c19b6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c19b6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsCategories/{userExperienceAnalyticsCategoryId}
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/bestPracticesMetrics
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/deviceBootPerformanceMetrics
```

## <a name="request-headers"></a><span data-ttu-id="c19b6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c19b6-119">Request headers</span></span>
|<span data-ttu-id="c19b6-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c19b6-120">Header</span></span>|<span data-ttu-id="c19b6-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c19b6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c19b6-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c19b6-122">Authorization</span></span>|<span data-ttu-id="c19b6-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c19b6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c19b6-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c19b6-124">Accept</span></span>|<span data-ttu-id="c19b6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c19b6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c19b6-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c19b6-126">Request body</span></span>
<span data-ttu-id="c19b6-127">В тексте запроса добавьте представление объекта [усерекспериенцеаналитикскатегори](../resources/intune-devices-userexperienceanalyticscategory.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c19b6-127">In the request body, supply a JSON representation for the [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>

<span data-ttu-id="c19b6-128">В следующей таблице приведены свойства, необходимые при создании [усерекспериенцеаналитикскатегори](../resources/intune-devices-userexperienceanalyticscategory.md).</span><span class="sxs-lookup"><span data-stu-id="c19b6-128">The following table shows the properties that are required when you create the [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md).</span></span>

|<span data-ttu-id="c19b6-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c19b6-129">Property</span></span>|<span data-ttu-id="c19b6-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c19b6-130">Type</span></span>|<span data-ttu-id="c19b6-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c19b6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c19b6-132">id</span><span class="sxs-lookup"><span data-stu-id="c19b6-132">id</span></span>|<span data-ttu-id="c19b6-133">String</span><span class="sxs-lookup"><span data-stu-id="c19b6-133">String</span></span>|<span data-ttu-id="c19b6-134">Уникальный идентификатор категории аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="c19b6-134">The unique identifier of the user experience analytics category.</span></span>|
|<span data-ttu-id="c19b6-135">овераллскоре</span><span class="sxs-lookup"><span data-stu-id="c19b6-135">overallScore</span></span>|<span data-ttu-id="c19b6-136">Int32</span><span class="sxs-lookup"><span data-stu-id="c19b6-136">Int32</span></span>|<span data-ttu-id="c19b6-137">Общий показатель категории аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="c19b6-137">The overall score of the user experience analytics category.</span></span>|
|<span data-ttu-id="c19b6-138">insights</span><span class="sxs-lookup"><span data-stu-id="c19b6-138">insights</span></span>|<span data-ttu-id="c19b6-139">Коллекция [усерекспериенцеаналитиксинсигхт](../resources/intune-devices-userexperienceanalyticsinsight.md)</span><span class="sxs-lookup"><span data-stu-id="c19b6-139">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="c19b6-140">Аналитика для категории аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="c19b6-140">The insights for the user experience analytics category.</span></span>|
|<span data-ttu-id="c19b6-141">state</span><span class="sxs-lookup"><span data-stu-id="c19b6-141">state</span></span>|[<span data-ttu-id="c19b6-142">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="c19b6-142">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="c19b6-143">Текущее состояние работоспособности категории аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="c19b6-143">The current health state of the user experience analytics category.</span></span> <span data-ttu-id="c19b6-144">Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="c19b6-144">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|



## <a name="response"></a><span data-ttu-id="c19b6-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="c19b6-145">Response</span></span>
<span data-ttu-id="c19b6-146">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [усерекспериенцеаналитикскатегори](../resources/intune-devices-userexperienceanalyticscategory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c19b6-146">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c19b6-147">Пример</span><span class="sxs-lookup"><span data-stu-id="c19b6-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="c19b6-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="c19b6-148">Request</span></span>
<span data-ttu-id="c19b6-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c19b6-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c19b6-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="c19b6-150">Response</span></span>
<span data-ttu-id="c19b6-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c19b6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






