---
title: Создание userExperienceAnalyticsMetric
description: Создание нового объекта userExperienceAnalyticsMetric.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6ad5b6320e257df35baf3011b8c19949bfe3118d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146204"
---
# <a name="create-userexperienceanalyticsmetric"></a><span data-ttu-id="b036f-103">Создание userExperienceAnalyticsMetric</span><span class="sxs-lookup"><span data-stu-id="b036f-103">Create userExperienceAnalyticsMetric</span></span>

<span data-ttu-id="b036f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b036f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b036f-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b036f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b036f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b036f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b036f-107">Создание нового [объекта userExperienceAnalyticsMetric.](../resources/intune-devices-userexperienceanalyticsmetric.md)</span><span class="sxs-lookup"><span data-stu-id="b036f-107">Create a new [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b036f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b036f-108">Prerequisites</span></span>
<span data-ttu-id="b036f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b036f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b036f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b036f-111">Permission type</span></span>|<span data-ttu-id="b036f-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b036f-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b036f-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b036f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b036f-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b036f-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b036f-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b036f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b036f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b036f-116">Not supported.</span></span>|
|<span data-ttu-id="b036f-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="b036f-117">Application</span></span>|<span data-ttu-id="b036f-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b036f-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b036f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b036f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsRegressionSummary/modelRegression
POST /deviceManagement/userExperienceAnalyticsRegressionSummary/manufacturerRegression
POST /deviceManagement/userExperienceAnalyticsRegressionSummary/operatingSystemRegression
POST /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/deviceBootPerformanceMetrics/metricValues
```

## <a name="request-headers"></a><span data-ttu-id="b036f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b036f-120">Request headers</span></span>
|<span data-ttu-id="b036f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b036f-121">Header</span></span>|<span data-ttu-id="b036f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b036f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b036f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b036f-123">Authorization</span></span>|<span data-ttu-id="b036f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b036f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b036f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b036f-125">Accept</span></span>|<span data-ttu-id="b036f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b036f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b036f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b036f-127">Request body</span></span>
<span data-ttu-id="b036f-128">В теле запроса поставляем представление JSON для объекта userExperienceAnalyticsMetric.</span><span class="sxs-lookup"><span data-stu-id="b036f-128">In the request body, supply a JSON representation for the userExperienceAnalyticsMetric object.</span></span>

<span data-ttu-id="b036f-129">В следующей таблице показаны свойства, необходимые при создании userExperienceAnalyticsMetric.</span><span class="sxs-lookup"><span data-stu-id="b036f-129">The following table shows the properties that are required when you create the userExperienceAnalyticsMetric.</span></span>

|<span data-ttu-id="b036f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b036f-130">Property</span></span>|<span data-ttu-id="b036f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b036f-131">Type</span></span>|<span data-ttu-id="b036f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b036f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b036f-133">id</span><span class="sxs-lookup"><span data-stu-id="b036f-133">id</span></span>|<span data-ttu-id="b036f-134">Строка</span><span class="sxs-lookup"><span data-stu-id="b036f-134">String</span></span>|<span data-ttu-id="b036f-135">Уникальный идентификатор метрики аналитики пользовательских интерфейсов.</span><span class="sxs-lookup"><span data-stu-id="b036f-135">The unique identifier of the user experience analytics metric.</span></span>|
|<span data-ttu-id="b036f-136">значение</span><span class="sxs-lookup"><span data-stu-id="b036f-136">value</span></span>|<span data-ttu-id="b036f-137">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="b036f-137">Double</span></span>|<span data-ttu-id="b036f-138">Значение метрики аналитики пользовательских интерфейсов.</span><span class="sxs-lookup"><span data-stu-id="b036f-138">The value of the user experience analytics metric.</span></span>|
|<span data-ttu-id="b036f-139">unit</span><span class="sxs-lookup"><span data-stu-id="b036f-139">unit</span></span>|<span data-ttu-id="b036f-140">Строка</span><span class="sxs-lookup"><span data-stu-id="b036f-140">String</span></span>|<span data-ttu-id="b036f-141">Единица метрики аналитики пользовательского опыта.</span><span class="sxs-lookup"><span data-stu-id="b036f-141">The unit of the user experience analytics metric.</span></span>|



## <a name="response"></a><span data-ttu-id="b036f-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="b036f-142">Response</span></span>
<span data-ttu-id="b036f-143">В случае успеха этот метод возвращает код отклика и `201 Created` [объект userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b036f-143">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b036f-144">Пример</span><span class="sxs-lookup"><span data-stu-id="b036f-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="b036f-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="b036f-145">Request</span></span>
<span data-ttu-id="b036f-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b036f-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsRegressionSummary/modelRegression
Content-type: application/json
Content-length: 128

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetric",
  "value": 1.6666666666666667,
  "unit": "Unit value"
}
```

### <a name="response"></a><span data-ttu-id="b036f-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="b036f-147">Response</span></span>
<span data-ttu-id="b036f-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b036f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 177

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetric",
  "id": "1371822e-822e-1371-2e82-71132e827113",
  "value": 1.6666666666666667,
  "unit": "Unit value"
}
```




