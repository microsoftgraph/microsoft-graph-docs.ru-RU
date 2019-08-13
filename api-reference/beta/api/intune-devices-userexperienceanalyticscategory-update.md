---
title: Обновление Усерекспериенцеаналитикскатегори
description: Обновление свойств объекта Усерекспериенцеаналитикскатегори.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f99c4bd2090f751b0a54df6ad408cda463266605
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36350490"
---
# <a name="update-userexperienceanalyticscategory"></a><span data-ttu-id="90915-103">Обновление Усерекспериенцеаналитикскатегори</span><span class="sxs-lookup"><span data-stu-id="90915-103">Update userExperienceAnalyticsCategory</span></span>

> <span data-ttu-id="90915-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90915-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="90915-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="90915-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90915-106">Обновление свойств объекта [усерекспериенцеаналитикскатегори](../resources/intune-devices-userexperienceanalyticscategory.md) .</span><span class="sxs-lookup"><span data-stu-id="90915-106">Update the properties of a [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="90915-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="90915-107">Prerequisites</span></span>
<span data-ttu-id="90915-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90915-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90915-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="90915-110">Permission type</span></span>|<span data-ttu-id="90915-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="90915-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90915-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="90915-112">Delegated (work or school account)</span></span>|<span data-ttu-id="90915-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90915-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="90915-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="90915-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90915-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90915-115">Not supported.</span></span>|
|<span data-ttu-id="90915-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="90915-116">Application</span></span>|<span data-ttu-id="90915-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90915-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="90915-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="90915-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsCategories/{userExperienceAnalyticsCategoryId}
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/bestPracticesMetrics
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/deviceBootPerformanceMetrics
```

## <a name="request-headers"></a><span data-ttu-id="90915-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="90915-119">Request headers</span></span>
|<span data-ttu-id="90915-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="90915-120">Header</span></span>|<span data-ttu-id="90915-121">Значение</span><span class="sxs-lookup"><span data-stu-id="90915-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="90915-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="90915-122">Authorization</span></span>|<span data-ttu-id="90915-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="90915-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="90915-124">Accept</span><span class="sxs-lookup"><span data-stu-id="90915-124">Accept</span></span>|<span data-ttu-id="90915-125">application/json</span><span class="sxs-lookup"><span data-stu-id="90915-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="90915-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="90915-126">Request body</span></span>
<span data-ttu-id="90915-127">В тексте запроса добавьте представление объекта [усерекспериенцеаналитикскатегори](../resources/intune-devices-userexperienceanalyticscategory.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="90915-127">In the request body, supply a JSON representation for the [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>

<span data-ttu-id="90915-128">В следующей таблице приведены свойства, необходимые при создании [усерекспериенцеаналитикскатегори](../resources/intune-devices-userexperienceanalyticscategory.md).</span><span class="sxs-lookup"><span data-stu-id="90915-128">The following table shows the properties that are required when you create the [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md).</span></span>

|<span data-ttu-id="90915-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="90915-129">Property</span></span>|<span data-ttu-id="90915-130">Тип</span><span class="sxs-lookup"><span data-stu-id="90915-130">Type</span></span>|<span data-ttu-id="90915-131">Описание</span><span class="sxs-lookup"><span data-stu-id="90915-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90915-132">id</span><span class="sxs-lookup"><span data-stu-id="90915-132">id</span></span>|<span data-ttu-id="90915-133">String</span><span class="sxs-lookup"><span data-stu-id="90915-133">String</span></span>|<span data-ttu-id="90915-134">Уникальный идентификатор категории аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="90915-134">The unique identifier of the user experience analytics category.</span></span>|
|<span data-ttu-id="90915-135">displayName</span><span class="sxs-lookup"><span data-stu-id="90915-135">displayName</span></span>|<span data-ttu-id="90915-136">Строка</span><span class="sxs-lookup"><span data-stu-id="90915-136">String</span></span>|<span data-ttu-id="90915-137">Имя категории аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="90915-137">The name of the user experience analytics category.</span></span>|
|<span data-ttu-id="90915-138">овераллскоре</span><span class="sxs-lookup"><span data-stu-id="90915-138">overallScore</span></span>|<span data-ttu-id="90915-139">Int32</span><span class="sxs-lookup"><span data-stu-id="90915-139">Int32</span></span>|<span data-ttu-id="90915-140">Общий показатель категории аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="90915-140">The overall score of the user experience analytics category.</span></span>|
|<span data-ttu-id="90915-141">insights</span><span class="sxs-lookup"><span data-stu-id="90915-141">insights</span></span>|<span data-ttu-id="90915-142">Коллекция [усерекспериенцеаналитиксинсигхт](../resources/intune-devices-userexperienceanalyticsinsight.md)</span><span class="sxs-lookup"><span data-stu-id="90915-142">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="90915-143">Аналитика для категории аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="90915-143">The insights for the user experience analytics category.</span></span>|



## <a name="response"></a><span data-ttu-id="90915-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="90915-144">Response</span></span>
<span data-ttu-id="90915-145">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [усерекспериенцеаналитикскатегори](../resources/intune-devices-userexperienceanalyticscategory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="90915-145">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90915-146">Пример</span><span class="sxs-lookup"><span data-stu-id="90915-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="90915-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="90915-147">Request</span></span>
<span data-ttu-id="90915-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="90915-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsCategories/{userExperienceAnalyticsCategoryId}
Content-type: application/json
Content-length: 484

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsCategory",
  "displayName": "Display Name value",
  "overallScore": 12,
  "insights": [
    {
      "@odata.type": "microsoft.graph.userExperienceAnalyticsInsight",
      "userExperienceAnalyticsMetricId": "User Experience Analytics Metric Id value",
      "insightId": "Insight Id value",
      "value": [
        {
          "@odata.type": "microsoft.graph.insightValueDouble"
        }
      ]
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="90915-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="90915-149">Response</span></span>
<span data-ttu-id="90915-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="90915-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 533

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsCategory",
  "id": "cfd28056-8056-cfd2-5680-d2cf5680d2cf",
  "displayName": "Display Name value",
  "overallScore": 12,
  "insights": [
    {
      "@odata.type": "microsoft.graph.userExperienceAnalyticsInsight",
      "userExperienceAnalyticsMetricId": "User Experience Analytics Metric Id value",
      "insightId": "Insight Id value",
      "value": [
        {
          "@odata.type": "microsoft.graph.insightValueDouble"
        }
      ]
    }
  ]
}
```






