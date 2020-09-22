---
title: Обновление Усерекспериенцеаналитиксапфеалсаппликатионперформанце
description: Обновление свойств объекта Усерекспериенцеаналитиксапфеалсаппликатионперформанце.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 38cf5bd0b6f0e88fec09a22edddb7ac88028f6a8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48017558"
---
# <a name="update-userexperienceanalyticsapphealthapplicationperformance"></a><span data-ttu-id="2149c-103">Обновление Усерекспериенцеаналитиксапфеалсаппликатионперформанце</span><span class="sxs-lookup"><span data-stu-id="2149c-103">Update userExperienceAnalyticsAppHealthApplicationPerformance</span></span>

<span data-ttu-id="2149c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2149c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2149c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2149c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2149c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2149c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2149c-107">Обновление свойств объекта [усерекспериенцеаналитиксапфеалсаппликатионперформанце](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) .</span><span class="sxs-lookup"><span data-stu-id="2149c-107">Update the properties of a [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2149c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2149c-108">Prerequisites</span></span>
<span data-ttu-id="2149c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2149c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2149c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2149c-111">Permission type</span></span>|<span data-ttu-id="2149c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2149c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2149c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2149c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2149c-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2149c-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="2149c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2149c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2149c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2149c-116">Not supported.</span></span>|
|<span data-ttu-id="2149c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2149c-117">Application</span></span>|<span data-ttu-id="2149c-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2149c-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2149c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2149c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformance/{userExperienceAnalyticsAppHealthApplicationPerformanceId}
```

## <a name="request-headers"></a><span data-ttu-id="2149c-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2149c-120">Request headers</span></span>
|<span data-ttu-id="2149c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2149c-121">Header</span></span>|<span data-ttu-id="2149c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2149c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2149c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2149c-123">Authorization</span></span>|<span data-ttu-id="2149c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2149c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2149c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2149c-125">Accept</span></span>|<span data-ttu-id="2149c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2149c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2149c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2149c-127">Request body</span></span>
<span data-ttu-id="2149c-128">В тексте запроса добавьте представление объекта [усерекспериенцеаналитиксапфеалсаппликатионперформанце](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2149c-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) object.</span></span>

<span data-ttu-id="2149c-129">В следующей таблице приведены свойства, необходимые при создании [усерекспериенцеаналитиксапфеалсаппликатионперформанце](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md).</span><span class="sxs-lookup"><span data-stu-id="2149c-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md).</span></span>

|<span data-ttu-id="2149c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2149c-130">Property</span></span>|<span data-ttu-id="2149c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2149c-131">Type</span></span>|<span data-ttu-id="2149c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2149c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2149c-133">id</span><span class="sxs-lookup"><span data-stu-id="2149c-133">id</span></span>|<span data-ttu-id="2149c-134">String</span><span class="sxs-lookup"><span data-stu-id="2149c-134">String</span></span>|<span data-ttu-id="2149c-135">Уникальный идентификатор объекта производительности приложения аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="2149c-135">The unique identifier of the user experience analytics app performance object.</span></span>|
|<span data-ttu-id="2149c-136">апфангкаунт</span><span class="sxs-lookup"><span data-stu-id="2149c-136">appHangCount</span></span>|<span data-ttu-id="2149c-137">Int32</span><span class="sxs-lookup"><span data-stu-id="2149c-137">Int32</span></span>|<span data-ttu-id="2149c-138">Число зависаний для приложения.</span><span class="sxs-lookup"><span data-stu-id="2149c-138">The number of hangs for the app.</span></span> <span data-ttu-id="2149c-139">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="2149c-139">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="2149c-140">апфеалсскоре</span><span class="sxs-lookup"><span data-stu-id="2149c-140">appHealthScore</span></span>|<span data-ttu-id="2149c-141">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="2149c-141">Double</span></span>|<span data-ttu-id="2149c-142">Оценка работоспособности приложения.</span><span class="sxs-lookup"><span data-stu-id="2149c-142">The health score of the app.</span></span> <span data-ttu-id="2149c-143">Допустимые значения — 1 79769313486232e308 E + 308 — 1 79769313486232e308 E + 308</span><span class="sxs-lookup"><span data-stu-id="2149c-143">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="2149c-144">апфеалсстатус</span><span class="sxs-lookup"><span data-stu-id="2149c-144">appHealthStatus</span></span>|<span data-ttu-id="2149c-145">String</span><span class="sxs-lookup"><span data-stu-id="2149c-145">String</span></span>|<span data-ttu-id="2149c-146">Общее состояние работоспособности приложения.</span><span class="sxs-lookup"><span data-stu-id="2149c-146">The overall health status of the app.</span></span>|
|<span data-ttu-id="2149c-147">аллоргшеалсскоре</span><span class="sxs-lookup"><span data-stu-id="2149c-147">allOrgsHealthScore</span></span>|<span data-ttu-id="2149c-148">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="2149c-148">Double</span></span>|<span data-ttu-id="2149c-149">Медианный показатель работоспособности приложения во всех организациях.</span><span class="sxs-lookup"><span data-stu-id="2149c-149">The median health score of the application across all organizations.</span></span> <span data-ttu-id="2149c-150">Допустимые значения — 1 79769313486232e308 E + 308 — 1 79769313486232e308 E + 308</span><span class="sxs-lookup"><span data-stu-id="2149c-150">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="2149c-151">активедевицекаунт</span><span class="sxs-lookup"><span data-stu-id="2149c-151">activeDeviceCount</span></span>|<span data-ttu-id="2149c-152">Int32</span><span class="sxs-lookup"><span data-stu-id="2149c-152">Int32</span></span>|<span data-ttu-id="2149c-153">Количество устройств, в которых приложение было активно.</span><span class="sxs-lookup"><span data-stu-id="2149c-153">The number of devices where the app has been active.</span></span> <span data-ttu-id="2149c-154">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="2149c-154">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="2149c-155">appName</span><span class="sxs-lookup"><span data-stu-id="2149c-155">appName</span></span>|<span data-ttu-id="2149c-156">String</span><span class="sxs-lookup"><span data-stu-id="2149c-156">String</span></span>|<span data-ttu-id="2149c-157">Имя приложения.</span><span class="sxs-lookup"><span data-stu-id="2149c-157">The name of the application.</span></span>|
|<span data-ttu-id="2149c-158">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="2149c-158">appDisplayName</span></span>|<span data-ttu-id="2149c-159">String</span><span class="sxs-lookup"><span data-stu-id="2149c-159">String</span></span>|<span data-ttu-id="2149c-160">Понятное имя приложения.</span><span class="sxs-lookup"><span data-stu-id="2149c-160">The friendly name of the application.</span></span>|
|<span data-ttu-id="2149c-161">апппублишер</span><span class="sxs-lookup"><span data-stu-id="2149c-161">appPublisher</span></span>|<span data-ttu-id="2149c-162">String</span><span class="sxs-lookup"><span data-stu-id="2149c-162">String</span></span>|<span data-ttu-id="2149c-163">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="2149c-163">The publisher of the application.</span></span>|
|<span data-ttu-id="2149c-164">аппусажедуратион</span><span class="sxs-lookup"><span data-stu-id="2149c-164">appUsageDuration</span></span>|<span data-ttu-id="2149c-165">Int32</span><span class="sxs-lookup"><span data-stu-id="2149c-165">Int32</span></span>|<span data-ttu-id="2149c-166">Общее время использования приложения в минутах.</span><span class="sxs-lookup"><span data-stu-id="2149c-166">The total usage time of the application in minutes.</span></span> <span data-ttu-id="2149c-167">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="2149c-167">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="2149c-168">аппкрашкаунт</span><span class="sxs-lookup"><span data-stu-id="2149c-168">appCrashCount</span></span>|<span data-ttu-id="2149c-169">Int32</span><span class="sxs-lookup"><span data-stu-id="2149c-169">Int32</span></span>|<span data-ttu-id="2149c-170">Число сбоев для приложения.</span><span class="sxs-lookup"><span data-stu-id="2149c-170">The number of crashes for the app.</span></span> <span data-ttu-id="2149c-171">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="2149c-171">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="2149c-172">меантиметофаилуреинминутес</span><span class="sxs-lookup"><span data-stu-id="2149c-172">meanTimeToFailureInMinutes</span></span>|<span data-ttu-id="2149c-173">Int32</span><span class="sxs-lookup"><span data-stu-id="2149c-173">Int32</span></span>|<span data-ttu-id="2149c-174">Среднее время до сбоя приложения в минутах.</span><span class="sxs-lookup"><span data-stu-id="2149c-174">The mean time to failure for the app in minutes.</span></span> <span data-ttu-id="2149c-175">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="2149c-175">Valid values -2147483648 to 2147483647</span></span>|



## <a name="response"></a><span data-ttu-id="2149c-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="2149c-176">Response</span></span>
<span data-ttu-id="2149c-177">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [усерекспериенцеаналитиксапфеалсаппликатионперформанце](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2149c-177">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2149c-178">Пример</span><span class="sxs-lookup"><span data-stu-id="2149c-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="2149c-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="2149c-179">Request</span></span>
<span data-ttu-id="2149c-180">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2149c-180">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2149c-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="2149c-181">Response</span></span>
<span data-ttu-id="2149c-p109">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2149c-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






