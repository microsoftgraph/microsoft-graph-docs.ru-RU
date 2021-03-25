---
title: Обновление userExperienceAnalyticsMetricHistory
description: Обновление свойств объекта userExperienceAnalyticsMetricHistory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ad5d90a7232e3e2723306f0e7ed0c7504b16d0de
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51159202"
---
# <a name="update-userexperienceanalyticsmetrichistory"></a><span data-ttu-id="a2a91-103">Обновление userExperienceAnalyticsMetricHistory</span><span class="sxs-lookup"><span data-stu-id="a2a91-103">Update userExperienceAnalyticsMetricHistory</span></span>

<span data-ttu-id="a2a91-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2a91-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a2a91-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2a91-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a2a91-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a2a91-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2a91-107">Обновление свойств объекта [userExperienceAnalyticsMetricHistory.](../resources/intune-devices-userexperienceanalyticsmetrichistory.md)</span><span class="sxs-lookup"><span data-stu-id="a2a91-107">Update the properties of a [userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a2a91-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a2a91-108">Prerequisites</span></span>
<span data-ttu-id="a2a91-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2a91-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2a91-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a2a91-111">Permission type</span></span>|<span data-ttu-id="a2a91-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a2a91-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2a91-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a2a91-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a2a91-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2a91-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a2a91-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a2a91-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2a91-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2a91-116">Not supported.</span></span>|
|<span data-ttu-id="a2a91-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="a2a91-117">Application</span></span>|<span data-ttu-id="a2a91-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2a91-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2a91-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a2a91-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsMetricHistory/{userExperienceAnalyticsMetricHistoryId}
PATCH /deviceManagement/userExperienceAnalyticsDeviceMetricHistory/{userExperienceAnalyticsMetricHistoryId}
```

## <a name="request-headers"></a><span data-ttu-id="a2a91-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a2a91-120">Request headers</span></span>
|<span data-ttu-id="a2a91-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a2a91-121">Header</span></span>|<span data-ttu-id="a2a91-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a2a91-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2a91-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2a91-123">Authorization</span></span>|<span data-ttu-id="a2a91-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a2a91-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2a91-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a2a91-125">Accept</span></span>|<span data-ttu-id="a2a91-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a2a91-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2a91-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a2a91-127">Request body</span></span>
<span data-ttu-id="a2a91-128">В теле запроса поставляем представление JSON для [объекта userExperienceAnalyticsMetricHistory.](../resources/intune-devices-userexperienceanalyticsmetrichistory.md)</span><span class="sxs-lookup"><span data-stu-id="a2a91-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) object.</span></span>

<span data-ttu-id="a2a91-129">В следующей таблице показаны свойства, необходимые при создании [userExperienceAnalyticsMetricHistory.](../resources/intune-devices-userexperienceanalyticsmetrichistory.md)</span><span class="sxs-lookup"><span data-stu-id="a2a91-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md).</span></span>

|<span data-ttu-id="a2a91-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a2a91-130">Property</span></span>|<span data-ttu-id="a2a91-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a2a91-131">Type</span></span>|<span data-ttu-id="a2a91-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a2a91-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2a91-133">id</span><span class="sxs-lookup"><span data-stu-id="a2a91-133">id</span></span>|<span data-ttu-id="a2a91-134">Строка</span><span class="sxs-lookup"><span data-stu-id="a2a91-134">String</span></span>|<span data-ttu-id="a2a91-135">Уникальный идентификатор метрики аналитики пользовательского опыта.</span><span class="sxs-lookup"><span data-stu-id="a2a91-135">The unique identifier of the user experience analytics metric history.</span></span>|
|<span data-ttu-id="a2a91-136">deviceId</span><span class="sxs-lookup"><span data-stu-id="a2a91-136">deviceId</span></span>|<span data-ttu-id="a2a91-137">String</span><span class="sxs-lookup"><span data-stu-id="a2a91-137">String</span></span>|<span data-ttu-id="a2a91-138">ID устройства аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="a2a91-138">The user experience analytics device id.</span></span>|
|<span data-ttu-id="a2a91-139">metricDateTime</span><span class="sxs-lookup"><span data-stu-id="a2a91-139">metricDateTime</span></span>|<span data-ttu-id="a2a91-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2a91-140">DateTimeOffset</span></span>|<span data-ttu-id="a2a91-141">Время даты даты аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="a2a91-141">The user experience analytics metric date time.</span></span>|
|<span data-ttu-id="a2a91-142">metricType</span><span class="sxs-lookup"><span data-stu-id="a2a91-142">metricType</span></span>|<span data-ttu-id="a2a91-143">Строка</span><span class="sxs-lookup"><span data-stu-id="a2a91-143">String</span></span>|<span data-ttu-id="a2a91-144">Тип метрики аналитики пользовательского опыта.</span><span class="sxs-lookup"><span data-stu-id="a2a91-144">The user experience analytics metric type.</span></span>|



## <a name="response"></a><span data-ttu-id="a2a91-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2a91-145">Response</span></span>
<span data-ttu-id="a2a91-146">В случае успеха этот метод возвращает код отклика и обновленный `200 OK` [объект userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a2a91-146">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2a91-147">Пример</span><span class="sxs-lookup"><span data-stu-id="a2a91-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="a2a91-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="a2a91-148">Request</span></span>
<span data-ttu-id="a2a91-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a2a91-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsMetricHistory/{userExperienceAnalyticsMetricHistoryId}
Content-type: application/json
Content-length: 208

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetricHistory",
  "deviceId": "Device Id value",
  "metricDateTime": "2017-01-01T00:00:28.4495993-08:00",
  "metricType": "Metric Type value"
}
```

### <a name="response"></a><span data-ttu-id="a2a91-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2a91-150">Response</span></span>
<span data-ttu-id="a2a91-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a2a91-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




