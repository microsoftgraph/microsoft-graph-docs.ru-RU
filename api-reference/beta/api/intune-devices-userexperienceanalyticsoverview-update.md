---
title: Обновление Усерекспериенцеаналитиксовервиев
description: Обновление свойств объекта Усерекспериенцеаналитиксовервиев.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: eb00499ea103b89dc45e1b5028858b0747f5163e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36350486"
---
# <a name="update-userexperienceanalyticsoverview"></a><span data-ttu-id="69f4e-103">Обновление Усерекспериенцеаналитиксовервиев</span><span class="sxs-lookup"><span data-stu-id="69f4e-103">Update userExperienceAnalyticsOverview</span></span>

> <span data-ttu-id="69f4e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69f4e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="69f4e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="69f4e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69f4e-106">Обновление свойств объекта [усерекспериенцеаналитиксовервиев](../resources/intune-devices-userexperienceanalyticsoverview.md) .</span><span class="sxs-lookup"><span data-stu-id="69f4e-106">Update the properties of a [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="69f4e-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="69f4e-107">Prerequisites</span></span>
<span data-ttu-id="69f4e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69f4e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69f4e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="69f4e-110">Permission type</span></span>|<span data-ttu-id="69f4e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="69f4e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69f4e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="69f4e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="69f4e-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69f4e-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="69f4e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="69f4e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69f4e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69f4e-115">Not supported.</span></span>|
|<span data-ttu-id="69f4e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="69f4e-116">Application</span></span>|<span data-ttu-id="69f4e-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69f4e-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="69f4e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="69f4e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsOverview
```

## <a name="request-headers"></a><span data-ttu-id="69f4e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="69f4e-119">Request headers</span></span>
|<span data-ttu-id="69f4e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="69f4e-120">Header</span></span>|<span data-ttu-id="69f4e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="69f4e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="69f4e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="69f4e-122">Authorization</span></span>|<span data-ttu-id="69f4e-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="69f4e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="69f4e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="69f4e-124">Accept</span></span>|<span data-ttu-id="69f4e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="69f4e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="69f4e-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="69f4e-126">Request body</span></span>
<span data-ttu-id="69f4e-127">В тексте запроса добавьте представление объекта [усерекспериенцеаналитиксовервиев](../resources/intune-devices-userexperienceanalyticsoverview.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="69f4e-127">In the request body, supply a JSON representation for the [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>

<span data-ttu-id="69f4e-128">В следующей таблице приведены свойства, необходимые при создании [усерекспериенцеаналитиксовервиев](../resources/intune-devices-userexperienceanalyticsoverview.md).</span><span class="sxs-lookup"><span data-stu-id="69f4e-128">The following table shows the properties that are required when you create the [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md).</span></span>

|<span data-ttu-id="69f4e-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="69f4e-129">Property</span></span>|<span data-ttu-id="69f4e-130">Тип</span><span class="sxs-lookup"><span data-stu-id="69f4e-130">Type</span></span>|<span data-ttu-id="69f4e-131">Описание</span><span class="sxs-lookup"><span data-stu-id="69f4e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69f4e-132">id</span><span class="sxs-lookup"><span data-stu-id="69f4e-132">id</span></span>|<span data-ttu-id="69f4e-133">String</span><span class="sxs-lookup"><span data-stu-id="69f4e-133">String</span></span>|<span data-ttu-id="69f4e-134">Уникальный идентификатор для обзора аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="69f4e-134">The unique identifier of the user experience analytics overview.</span></span>|
|<span data-ttu-id="69f4e-135">овераллскоре</span><span class="sxs-lookup"><span data-stu-id="69f4e-135">overallScore</span></span>|<span data-ttu-id="69f4e-136">Int32</span><span class="sxs-lookup"><span data-stu-id="69f4e-136">Int32</span></span>|<span data-ttu-id="69f4e-137">Общий показатель аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="69f4e-137">The user experience analytics overall score.</span></span>|
|<span data-ttu-id="69f4e-138">девицебутперформанцеовераллскоре</span><span class="sxs-lookup"><span data-stu-id="69f4e-138">deviceBootPerformanceOverallScore</span></span>|<span data-ttu-id="69f4e-139">Int32</span><span class="sxs-lookup"><span data-stu-id="69f4e-139">Int32</span></span>|<span data-ttu-id="69f4e-140">Общая оценка производительности при загрузке устройства Analytics.</span><span class="sxs-lookup"><span data-stu-id="69f4e-140">The user experience analytics device boot performance overall score.</span></span>|
|<span data-ttu-id="69f4e-141">бестпрактицесовераллскоре</span><span class="sxs-lookup"><span data-stu-id="69f4e-141">bestPracticesOverallScore</span></span>|<span data-ttu-id="69f4e-142">Int32</span><span class="sxs-lookup"><span data-stu-id="69f4e-142">Int32</span></span>|<span data-ttu-id="69f4e-143">Общая оценка рекомендаций по анализу пользовательских интерфейсов.</span><span class="sxs-lookup"><span data-stu-id="69f4e-143">The user experience analytics best practices overall score.</span></span>|
|<span data-ttu-id="69f4e-144">insights</span><span class="sxs-lookup"><span data-stu-id="69f4e-144">insights</span></span>|<span data-ttu-id="69f4e-145">Коллекция [усерекспериенцеаналитиксинсигхт](../resources/intune-devices-userexperienceanalyticsinsight.md)</span><span class="sxs-lookup"><span data-stu-id="69f4e-145">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="69f4e-146">Аналитика взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="69f4e-146">The user experience analytics insights.</span></span>|



## <a name="response"></a><span data-ttu-id="69f4e-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="69f4e-147">Response</span></span>
<span data-ttu-id="69f4e-148">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [усерекспериенцеаналитиксовервиев](../resources/intune-devices-userexperienceanalyticsoverview.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="69f4e-148">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69f4e-149">Пример</span><span class="sxs-lookup"><span data-stu-id="69f4e-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="69f4e-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="69f4e-150">Request</span></span>
<span data-ttu-id="69f4e-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="69f4e-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsOverview
Content-type: application/json
Content-length: 522

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
      "value": [
        {
          "@odata.type": "microsoft.graph.insightValueDouble"
        }
      ]
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="69f4e-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="69f4e-152">Response</span></span>
<span data-ttu-id="69f4e-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="69f4e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 571

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
      "value": [
        {
          "@odata.type": "microsoft.graph.insightValueDouble"
        }
      ]
    }
  ]
}
```






