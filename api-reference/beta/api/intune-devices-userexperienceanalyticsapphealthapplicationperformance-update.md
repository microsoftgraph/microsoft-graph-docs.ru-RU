---
title: Обновление userExperienceAnalyticsAppHealthApplicationPerformance
description: Обновление свойств объекта userExperienceAnalyticsAppHealthApplicationPerformance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 99ffe6141c124e8de8ecd1a6a7fdf362b9cf6ff9
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51158103"
---
# <a name="update-userexperienceanalyticsapphealthapplicationperformance"></a><span data-ttu-id="29b91-103">Обновление userExperienceAnalyticsAppHealthApplicationPerformance</span><span class="sxs-lookup"><span data-stu-id="29b91-103">Update userExperienceAnalyticsAppHealthApplicationPerformance</span></span>

<span data-ttu-id="29b91-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29b91-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="29b91-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="29b91-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="29b91-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="29b91-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="29b91-107">Обновление свойств объекта [userExperienceAnalyticsAppHealthApplicationPerformance.](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md)</span><span class="sxs-lookup"><span data-stu-id="29b91-107">Update the properties of a [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="29b91-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="29b91-108">Prerequisites</span></span>
<span data-ttu-id="29b91-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29b91-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29b91-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="29b91-111">Permission type</span></span>|<span data-ttu-id="29b91-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="29b91-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="29b91-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="29b91-113">Delegated (work or school account)</span></span>|<span data-ttu-id="29b91-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29b91-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="29b91-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="29b91-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="29b91-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="29b91-116">Not supported.</span></span>|
|<span data-ttu-id="29b91-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="29b91-117">Application</span></span>|<span data-ttu-id="29b91-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29b91-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="29b91-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="29b91-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformance/{userExperienceAnalyticsAppHealthApplicationPerformanceId}
```

## <a name="request-headers"></a><span data-ttu-id="29b91-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="29b91-120">Request headers</span></span>
|<span data-ttu-id="29b91-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="29b91-121">Header</span></span>|<span data-ttu-id="29b91-122">Значение</span><span class="sxs-lookup"><span data-stu-id="29b91-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="29b91-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="29b91-123">Authorization</span></span>|<span data-ttu-id="29b91-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="29b91-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="29b91-125">Accept</span><span class="sxs-lookup"><span data-stu-id="29b91-125">Accept</span></span>|<span data-ttu-id="29b91-126">application/json</span><span class="sxs-lookup"><span data-stu-id="29b91-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="29b91-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="29b91-127">Request body</span></span>
<span data-ttu-id="29b91-128">В теле запроса поставляем представление JSON для [объекта userExperienceAnalyticsAppHealthApplicationPerformance.](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md)</span><span class="sxs-lookup"><span data-stu-id="29b91-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) object.</span></span>

<span data-ttu-id="29b91-129">В следующей таблице показаны свойства, необходимые при создании [userExperienceAnalyticsAppHealthApplicationPerformance.](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md)</span><span class="sxs-lookup"><span data-stu-id="29b91-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md).</span></span>

|<span data-ttu-id="29b91-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="29b91-130">Property</span></span>|<span data-ttu-id="29b91-131">Тип</span><span class="sxs-lookup"><span data-stu-id="29b91-131">Type</span></span>|<span data-ttu-id="29b91-132">Описание</span><span class="sxs-lookup"><span data-stu-id="29b91-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29b91-133">id</span><span class="sxs-lookup"><span data-stu-id="29b91-133">id</span></span>|<span data-ttu-id="29b91-134">Строка</span><span class="sxs-lookup"><span data-stu-id="29b91-134">String</span></span>|<span data-ttu-id="29b91-135">Уникальный идентификатор объекта производительности приложения для аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="29b91-135">The unique identifier of the user experience analytics app performance object.</span></span>|
|<span data-ttu-id="29b91-136">appHangCount</span><span class="sxs-lookup"><span data-stu-id="29b91-136">appHangCount</span></span>|<span data-ttu-id="29b91-137">Int32</span><span class="sxs-lookup"><span data-stu-id="29b91-137">Int32</span></span>|<span data-ttu-id="29b91-138">Количество зависает для приложения.</span><span class="sxs-lookup"><span data-stu-id="29b91-138">The number of hangs for the app.</span></span> <span data-ttu-id="29b91-139">Допустимые значения -2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="29b91-139">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="29b91-140">appHealthScore</span><span class="sxs-lookup"><span data-stu-id="29b91-140">appHealthScore</span></span>|<span data-ttu-id="29b91-141">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="29b91-141">Double</span></span>|<span data-ttu-id="29b91-142">Оценка состояния здоровья приложения.</span><span class="sxs-lookup"><span data-stu-id="29b91-142">The health score of the app.</span></span> <span data-ttu-id="29b91-143">Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308</span><span class="sxs-lookup"><span data-stu-id="29b91-143">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="29b91-144">appHealthStatus</span><span class="sxs-lookup"><span data-stu-id="29b91-144">appHealthStatus</span></span>|<span data-ttu-id="29b91-145">Строка</span><span class="sxs-lookup"><span data-stu-id="29b91-145">String</span></span>|<span data-ttu-id="29b91-146">Общее состояние здоровья приложения.</span><span class="sxs-lookup"><span data-stu-id="29b91-146">The overall health status of the app.</span></span>|
|<span data-ttu-id="29b91-147">allOrgsHealthScore</span><span class="sxs-lookup"><span data-stu-id="29b91-147">allOrgsHealthScore</span></span>|<span data-ttu-id="29b91-148">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="29b91-148">Double</span></span>|<span data-ttu-id="29b91-149">Медиана оценка состояния здоровья приложения во всех организациях.</span><span class="sxs-lookup"><span data-stu-id="29b91-149">The median health score of the application across all organizations.</span></span> <span data-ttu-id="29b91-150">Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308</span><span class="sxs-lookup"><span data-stu-id="29b91-150">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="29b91-151">activeDeviceCount</span><span class="sxs-lookup"><span data-stu-id="29b91-151">activeDeviceCount</span></span>|<span data-ttu-id="29b91-152">Int32</span><span class="sxs-lookup"><span data-stu-id="29b91-152">Int32</span></span>|<span data-ttu-id="29b91-153">Количество устройств, на которых приложение было активным.</span><span class="sxs-lookup"><span data-stu-id="29b91-153">The number of devices where the app has been active.</span></span> <span data-ttu-id="29b91-154">Допустимые значения -2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="29b91-154">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="29b91-155">appName</span><span class="sxs-lookup"><span data-stu-id="29b91-155">appName</span></span>|<span data-ttu-id="29b91-156">String</span><span class="sxs-lookup"><span data-stu-id="29b91-156">String</span></span>|<span data-ttu-id="29b91-157">Имя приложения.</span><span class="sxs-lookup"><span data-stu-id="29b91-157">The name of the application.</span></span>|
|<span data-ttu-id="29b91-158">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="29b91-158">appDisplayName</span></span>|<span data-ttu-id="29b91-159">String</span><span class="sxs-lookup"><span data-stu-id="29b91-159">String</span></span>|<span data-ttu-id="29b91-160">Удобное имя приложения.</span><span class="sxs-lookup"><span data-stu-id="29b91-160">The friendly name of the application.</span></span>|
|<span data-ttu-id="29b91-161">appPublisher</span><span class="sxs-lookup"><span data-stu-id="29b91-161">appPublisher</span></span>|<span data-ttu-id="29b91-162">Строка</span><span class="sxs-lookup"><span data-stu-id="29b91-162">String</span></span>|<span data-ttu-id="29b91-163">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="29b91-163">The publisher of the application.</span></span>|
|<span data-ttu-id="29b91-164">appUsageDuration</span><span class="sxs-lookup"><span data-stu-id="29b91-164">appUsageDuration</span></span>|<span data-ttu-id="29b91-165">Int32</span><span class="sxs-lookup"><span data-stu-id="29b91-165">Int32</span></span>|<span data-ttu-id="29b91-166">Общее время использования приложения в минутах.</span><span class="sxs-lookup"><span data-stu-id="29b91-166">The total usage time of the application in minutes.</span></span> <span data-ttu-id="29b91-167">Допустимые значения -2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="29b91-167">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="29b91-168">appCrashCount</span><span class="sxs-lookup"><span data-stu-id="29b91-168">appCrashCount</span></span>|<span data-ttu-id="29b91-169">Int32</span><span class="sxs-lookup"><span data-stu-id="29b91-169">Int32</span></span>|<span data-ttu-id="29b91-170">Количество сбоей для приложения.</span><span class="sxs-lookup"><span data-stu-id="29b91-170">The number of crashes for the app.</span></span> <span data-ttu-id="29b91-171">Допустимые значения -2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="29b91-171">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="29b91-172">meanTimeToFailureInMinutes</span><span class="sxs-lookup"><span data-stu-id="29b91-172">meanTimeToFailureInMinutes</span></span>|<span data-ttu-id="29b91-173">Int32</span><span class="sxs-lookup"><span data-stu-id="29b91-173">Int32</span></span>|<span data-ttu-id="29b91-174">Время сбоя для приложения в минутах.</span><span class="sxs-lookup"><span data-stu-id="29b91-174">The mean time to failure for the app in minutes.</span></span> <span data-ttu-id="29b91-175">Допустимые значения -2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="29b91-175">Valid values -2147483648 to 2147483647</span></span>|



## <a name="response"></a><span data-ttu-id="29b91-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="29b91-176">Response</span></span>
<span data-ttu-id="29b91-177">В случае успеха этот метод возвращает код отклика и обновленный объект `200 OK` [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="29b91-177">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29b91-178">Пример</span><span class="sxs-lookup"><span data-stu-id="29b91-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="29b91-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="29b91-179">Request</span></span>
<span data-ttu-id="29b91-180">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="29b91-180">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformance/{userExperienceAnalyticsAppHealthApplicationPerformanceId}
Content-type: application/json
Content-length: 473

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthApplicationPerformance",
  "appHangCount": 12,
  "appHealthScore": 4.666666666666667,
  "appHealthStatus": "App Health Status value",
  "allOrgsHealthScore": 6.0,
  "activeDeviceCount": 1,
  "appName": "App Name value",
  "appDisplayName": "App Display Name value",
  "appPublisher": "App Publisher value",
  "appUsageDuration": 0,
  "appCrashCount": 13,
  "meanTimeToFailureInMinutes": 10
}
```

### <a name="response"></a><span data-ttu-id="29b91-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="29b91-181">Response</span></span>
<span data-ttu-id="29b91-p109">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="29b91-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 522

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthApplicationPerformance",
  "id": "c7962a87-2a87-c796-872a-96c7872a96c7",
  "appHangCount": 12,
  "appHealthScore": 4.666666666666667,
  "appHealthStatus": "App Health Status value",
  "allOrgsHealthScore": 6.0,
  "activeDeviceCount": 1,
  "appName": "App Name value",
  "appDisplayName": "App Display Name value",
  "appPublisher": "App Publisher value",
  "appUsageDuration": 0,
  "appCrashCount": 13,
  "meanTimeToFailureInMinutes": 10
}
```




