---
title: Создание userExperienceAnalyticsMetricHistory
description: Создание нового объекта userExperienceAnalyticsMetricHistory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f5160db6d8a589eaef946e52675e2cb9d2d3e943
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51159244"
---
# <a name="create-userexperienceanalyticsmetrichistory"></a><span data-ttu-id="e0904-103">Создание userExperienceAnalyticsMetricHistory</span><span class="sxs-lookup"><span data-stu-id="e0904-103">Create userExperienceAnalyticsMetricHistory</span></span>

<span data-ttu-id="e0904-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0904-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e0904-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0904-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e0904-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e0904-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0904-107">Создание нового [объекта userExperienceAnalyticsMetricHistory.](../resources/intune-devices-userexperienceanalyticsmetrichistory.md)</span><span class="sxs-lookup"><span data-stu-id="e0904-107">Create a new [userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e0904-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e0904-108">Prerequisites</span></span>
<span data-ttu-id="e0904-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0904-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0904-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e0904-111">Permission type</span></span>|<span data-ttu-id="e0904-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e0904-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e0904-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e0904-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e0904-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0904-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e0904-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e0904-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e0904-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0904-116">Not supported.</span></span>|
|<span data-ttu-id="e0904-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="e0904-117">Application</span></span>|<span data-ttu-id="e0904-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0904-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e0904-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e0904-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsMetricHistory
POST /deviceManagement/userExperienceAnalyticsDeviceMetricHistory
```

## <a name="request-headers"></a><span data-ttu-id="e0904-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e0904-120">Request headers</span></span>
|<span data-ttu-id="e0904-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e0904-121">Header</span></span>|<span data-ttu-id="e0904-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e0904-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e0904-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0904-123">Authorization</span></span>|<span data-ttu-id="e0904-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e0904-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e0904-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e0904-125">Accept</span></span>|<span data-ttu-id="e0904-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e0904-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0904-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e0904-127">Request body</span></span>
<span data-ttu-id="e0904-128">В теле запроса поставляем представление JSON для объекта userExperienceAnalyticsMetricHistory.</span><span class="sxs-lookup"><span data-stu-id="e0904-128">In the request body, supply a JSON representation for the userExperienceAnalyticsMetricHistory object.</span></span>

<span data-ttu-id="e0904-129">В следующей таблице показаны свойства, необходимые при создании userExperienceAnalyticsMetricHistory.</span><span class="sxs-lookup"><span data-stu-id="e0904-129">The following table shows the properties that are required when you create the userExperienceAnalyticsMetricHistory.</span></span>

|<span data-ttu-id="e0904-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e0904-130">Property</span></span>|<span data-ttu-id="e0904-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e0904-131">Type</span></span>|<span data-ttu-id="e0904-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e0904-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0904-133">id</span><span class="sxs-lookup"><span data-stu-id="e0904-133">id</span></span>|<span data-ttu-id="e0904-134">Строка</span><span class="sxs-lookup"><span data-stu-id="e0904-134">String</span></span>|<span data-ttu-id="e0904-135">Уникальный идентификатор метрики аналитики пользовательского опыта.</span><span class="sxs-lookup"><span data-stu-id="e0904-135">The unique identifier of the user experience analytics metric history.</span></span>|
|<span data-ttu-id="e0904-136">deviceId</span><span class="sxs-lookup"><span data-stu-id="e0904-136">deviceId</span></span>|<span data-ttu-id="e0904-137">String</span><span class="sxs-lookup"><span data-stu-id="e0904-137">String</span></span>|<span data-ttu-id="e0904-138">ID устройства аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="e0904-138">The user experience analytics device id.</span></span>|
|<span data-ttu-id="e0904-139">metricDateTime</span><span class="sxs-lookup"><span data-stu-id="e0904-139">metricDateTime</span></span>|<span data-ttu-id="e0904-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0904-140">DateTimeOffset</span></span>|<span data-ttu-id="e0904-141">Время даты даты аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="e0904-141">The user experience analytics metric date time.</span></span>|
|<span data-ttu-id="e0904-142">metricType</span><span class="sxs-lookup"><span data-stu-id="e0904-142">metricType</span></span>|<span data-ttu-id="e0904-143">Строка</span><span class="sxs-lookup"><span data-stu-id="e0904-143">String</span></span>|<span data-ttu-id="e0904-144">Тип метрики аналитики пользовательского опыта.</span><span class="sxs-lookup"><span data-stu-id="e0904-144">The user experience analytics metric type.</span></span>|



## <a name="response"></a><span data-ttu-id="e0904-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="e0904-145">Response</span></span>
<span data-ttu-id="e0904-146">В случае успеха этот метод возвращает код отклика и `201 Created` [объект userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e0904-146">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0904-147">Пример</span><span class="sxs-lookup"><span data-stu-id="e0904-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="e0904-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="e0904-148">Request</span></span>
<span data-ttu-id="e0904-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e0904-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsMetricHistory
Content-type: application/json
Content-length: 208

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetricHistory",
  "deviceId": "Device Id value",
  "metricDateTime": "2017-01-01T00:00:28.4495993-08:00",
  "metricType": "Metric Type value"
}
```

### <a name="response"></a><span data-ttu-id="e0904-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="e0904-150">Response</span></span>
<span data-ttu-id="e0904-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e0904-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 257

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetricHistory",
  "id": "2b6d6456-6456-2b6d-5664-6d2b56646d2b",
  "deviceId": "Device Id value",
  "metricDateTime": "2017-01-01T00:00:28.4495993-08:00",
  "metricType": "Metric Type value"
}
```




