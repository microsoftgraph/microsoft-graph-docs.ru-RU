---
title: Обновление Усерекспериенцеаналитиксметрик
description: Обновление свойств объекта Усерекспериенцеаналитиксметрик.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 43502ab7807a3e821011faa440704a11f9e3c9d4
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36350488"
---
# <a name="update-userexperienceanalyticsmetric"></a><span data-ttu-id="82b21-103">Обновление Усерекспериенцеаналитиксметрик</span><span class="sxs-lookup"><span data-stu-id="82b21-103">Update userExperienceAnalyticsMetric</span></span>

> <span data-ttu-id="82b21-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82b21-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="82b21-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="82b21-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82b21-106">Обновление свойств объекта [усерекспериенцеаналитиксметрик](../resources/intune-devices-userexperienceanalyticsmetric.md) .</span><span class="sxs-lookup"><span data-stu-id="82b21-106">Update the properties of a [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="82b21-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="82b21-107">Prerequisites</span></span>
<span data-ttu-id="82b21-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82b21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82b21-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="82b21-110">Permission type</span></span>|<span data-ttu-id="82b21-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="82b21-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82b21-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="82b21-112">Delegated (work or school account)</span></span>|<span data-ttu-id="82b21-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82b21-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="82b21-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="82b21-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82b21-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82b21-115">Not supported.</span></span>|
|<span data-ttu-id="82b21-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="82b21-116">Application</span></span>|<span data-ttu-id="82b21-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82b21-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="82b21-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="82b21-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/deviceBootPerformanceMetrics/metricValues/{userExperienceAnalyticsMetricId}
```

## <a name="request-headers"></a><span data-ttu-id="82b21-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="82b21-119">Request headers</span></span>
|<span data-ttu-id="82b21-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="82b21-120">Header</span></span>|<span data-ttu-id="82b21-121">Значение</span><span class="sxs-lookup"><span data-stu-id="82b21-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="82b21-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="82b21-122">Authorization</span></span>|<span data-ttu-id="82b21-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="82b21-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="82b21-124">Accept</span><span class="sxs-lookup"><span data-stu-id="82b21-124">Accept</span></span>|<span data-ttu-id="82b21-125">application/json</span><span class="sxs-lookup"><span data-stu-id="82b21-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="82b21-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="82b21-126">Request body</span></span>
<span data-ttu-id="82b21-127">В тексте запроса добавьте представление объекта [усерекспериенцеаналитиксметрик](../resources/intune-devices-userexperienceanalyticsmetric.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="82b21-127">In the request body, supply a JSON representation for the [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) object.</span></span>

<span data-ttu-id="82b21-128">В следующей таблице приведены свойства, необходимые при создании [усерекспериенцеаналитиксметрик](../resources/intune-devices-userexperienceanalyticsmetric.md).</span><span class="sxs-lookup"><span data-stu-id="82b21-128">The following table shows the properties that are required when you create the [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md).</span></span>

|<span data-ttu-id="82b21-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="82b21-129">Property</span></span>|<span data-ttu-id="82b21-130">Тип</span><span class="sxs-lookup"><span data-stu-id="82b21-130">Type</span></span>|<span data-ttu-id="82b21-131">Описание</span><span class="sxs-lookup"><span data-stu-id="82b21-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82b21-132">id</span><span class="sxs-lookup"><span data-stu-id="82b21-132">id</span></span>|<span data-ttu-id="82b21-133">String</span><span class="sxs-lookup"><span data-stu-id="82b21-133">String</span></span>|<span data-ttu-id="82b21-134">Уникальный идентификатор метрики аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="82b21-134">The unique identifier of the user experience analytics metric.</span></span>|
|<span data-ttu-id="82b21-135">displayName</span><span class="sxs-lookup"><span data-stu-id="82b21-135">displayName</span></span>|<span data-ttu-id="82b21-136">Строка</span><span class="sxs-lookup"><span data-stu-id="82b21-136">String</span></span>|<span data-ttu-id="82b21-137">Имя метрики аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="82b21-137">The name of the user experience analytics metric.</span></span>|
|<span data-ttu-id="82b21-138">значение</span><span class="sxs-lookup"><span data-stu-id="82b21-138">value</span></span>|<span data-ttu-id="82b21-139">Двойное</span><span class="sxs-lookup"><span data-stu-id="82b21-139">Double</span></span>|<span data-ttu-id="82b21-140">Значение метрики аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="82b21-140">The value of the user experience analytics metric.</span></span>|
|<span data-ttu-id="82b21-141">устройств</span><span class="sxs-lookup"><span data-stu-id="82b21-141">unit</span></span>|<span data-ttu-id="82b21-142">String</span><span class="sxs-lookup"><span data-stu-id="82b21-142">String</span></span>|<span data-ttu-id="82b21-143">Единица измерения показателя взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="82b21-143">The unit of the user experience analytics metric.</span></span>|



## <a name="response"></a><span data-ttu-id="82b21-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="82b21-144">Response</span></span>
<span data-ttu-id="82b21-145">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [усерекспериенцеаналитиксметрик](../resources/intune-devices-userexperienceanalyticsmetric.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="82b21-145">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82b21-146">Пример</span><span class="sxs-lookup"><span data-stu-id="82b21-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="82b21-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="82b21-147">Request</span></span>
<span data-ttu-id="82b21-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="82b21-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/deviceBootPerformanceMetrics/metricValues/{userExperienceAnalyticsMetricId}
Content-type: application/json
Content-length: 187

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetric",
  "displayName": "Display Name value",
  "value": "<Unknown Primitive Type Edm.Double>",
  "unit": "Unit value"
}
```

### <a name="response"></a><span data-ttu-id="82b21-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="82b21-149">Response</span></span>
<span data-ttu-id="82b21-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="82b21-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 236

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetric",
  "id": "1371822e-822e-1371-2e82-71132e827113",
  "displayName": "Display Name value",
  "value": "<Unknown Primitive Type Edm.Double>",
  "unit": "Unit value"
}
```






