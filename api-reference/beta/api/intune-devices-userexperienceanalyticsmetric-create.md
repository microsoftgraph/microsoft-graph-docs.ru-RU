---
title: Создание Усерекспериенцеаналитиксметрик
description: Создание нового объекта Усерекспериенцеаналитиксметрик.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b9e8ca95bcb11d26212f0248fcced244d6edbc9d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42468238"
---
# <a name="create-userexperienceanalyticsmetric"></a><span data-ttu-id="dd739-103">Создание Усерекспериенцеаналитиксметрик</span><span class="sxs-lookup"><span data-stu-id="dd739-103">Create userExperienceAnalyticsMetric</span></span>

<span data-ttu-id="dd739-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="dd739-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dd739-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd739-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dd739-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dd739-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd739-107">Создание нового объекта [усерекспериенцеаналитиксметрик](../resources/intune-devices-userexperienceanalyticsmetric.md) .</span><span class="sxs-lookup"><span data-stu-id="dd739-107">Create a new [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dd739-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="dd739-108">Prerequisites</span></span>
<span data-ttu-id="dd739-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd739-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd739-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dd739-111">Permission type</span></span>|<span data-ttu-id="dd739-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dd739-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dd739-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dd739-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dd739-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd739-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="dd739-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dd739-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dd739-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd739-116">Not supported.</span></span>|
|<span data-ttu-id="dd739-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dd739-117">Application</span></span>|<span data-ttu-id="dd739-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd739-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dd739-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dd739-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="dd739-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="dd739-120">Request headers</span></span>
|<span data-ttu-id="dd739-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dd739-121">Header</span></span>|<span data-ttu-id="dd739-122">Значение</span><span class="sxs-lookup"><span data-stu-id="dd739-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dd739-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd739-123">Authorization</span></span>|<span data-ttu-id="dd739-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dd739-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dd739-125">Accept</span><span class="sxs-lookup"><span data-stu-id="dd739-125">Accept</span></span>|<span data-ttu-id="dd739-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dd739-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd739-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dd739-127">Request body</span></span>
<span data-ttu-id="dd739-128">В тексте запроса добавьте представление объекта Усерекспериенцеаналитиксметрик в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dd739-128">In the request body, supply a JSON representation for the userExperienceAnalyticsMetric object.</span></span>

<span data-ttu-id="dd739-129">В следующей таблице приведены свойства, необходимые при создании Усерекспериенцеаналитиксметрик.</span><span class="sxs-lookup"><span data-stu-id="dd739-129">The following table shows the properties that are required when you create the userExperienceAnalyticsMetric.</span></span>

|<span data-ttu-id="dd739-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="dd739-130">Property</span></span>|<span data-ttu-id="dd739-131">Тип</span><span class="sxs-lookup"><span data-stu-id="dd739-131">Type</span></span>|<span data-ttu-id="dd739-132">Описание</span><span class="sxs-lookup"><span data-stu-id="dd739-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd739-133">id</span><span class="sxs-lookup"><span data-stu-id="dd739-133">id</span></span>|<span data-ttu-id="dd739-134">String</span><span class="sxs-lookup"><span data-stu-id="dd739-134">String</span></span>|<span data-ttu-id="dd739-135">Уникальный идентификатор метрики аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="dd739-135">The unique identifier of the user experience analytics metric.</span></span>|
|<span data-ttu-id="dd739-136">значение</span><span class="sxs-lookup"><span data-stu-id="dd739-136">value</span></span>|<span data-ttu-id="dd739-137">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="dd739-137">Double</span></span>|<span data-ttu-id="dd739-138">Значение метрики аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="dd739-138">The value of the user experience analytics metric.</span></span>|
|<span data-ttu-id="dd739-139">устройств</span><span class="sxs-lookup"><span data-stu-id="dd739-139">unit</span></span>|<span data-ttu-id="dd739-140">String</span><span class="sxs-lookup"><span data-stu-id="dd739-140">String</span></span>|<span data-ttu-id="dd739-141">Единица измерения показателя взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="dd739-141">The unit of the user experience analytics metric.</span></span>|



## <a name="response"></a><span data-ttu-id="dd739-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd739-142">Response</span></span>
<span data-ttu-id="dd739-143">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [усерекспериенцеаналитиксметрик](../resources/intune-devices-userexperienceanalyticsmetric.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dd739-143">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd739-144">Пример</span><span class="sxs-lookup"><span data-stu-id="dd739-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="dd739-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="dd739-145">Request</span></span>
<span data-ttu-id="dd739-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dd739-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsRegressionSummary/modelRegression
Content-type: application/json
Content-length: 147

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetric",
  "value": "<Unknown Primitive Type Edm.Double>",
  "unit": "Unit value"
}
```

### <a name="response"></a><span data-ttu-id="dd739-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd739-147">Response</span></span>
<span data-ttu-id="dd739-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dd739-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 196

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetric",
  "id": "1371822e-822e-1371-2e82-71132e827113",
  "value": "<Unknown Primitive Type Edm.Double>",
  "unit": "Unit value"
}
```





