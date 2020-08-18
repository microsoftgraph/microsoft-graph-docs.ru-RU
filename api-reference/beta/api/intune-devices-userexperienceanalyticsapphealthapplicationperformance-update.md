---
title: Обновление Усерекспериенцеаналитиксапфеалсаппликатионперформанце
description: Обновление свойств объекта Усерекспериенцеаналитиксапфеалсаппликатионперформанце.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3e845c25f1174b36941f22c249f91d365a83a590
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/18/2020
ms.locfileid: "46793526"
---
# <a name="update-userexperienceanalyticsapphealthapplicationperformance"></a><span data-ttu-id="778b9-103">Обновление Усерекспериенцеаналитиксапфеалсаппликатионперформанце</span><span class="sxs-lookup"><span data-stu-id="778b9-103">Update userExperienceAnalyticsAppHealthApplicationPerformance</span></span>

<span data-ttu-id="778b9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="778b9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="778b9-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="778b9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="778b9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="778b9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="778b9-107">Обновление свойств объекта [усерекспериенцеаналитиксапфеалсаппликатионперформанце](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) .</span><span class="sxs-lookup"><span data-stu-id="778b9-107">Update the properties of a [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="778b9-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="778b9-108">Prerequisites</span></span>
<span data-ttu-id="778b9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="778b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="778b9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="778b9-111">Permission type</span></span>|<span data-ttu-id="778b9-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="778b9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="778b9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="778b9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="778b9-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="778b9-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="778b9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="778b9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="778b9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="778b9-116">Not supported.</span></span>|
|<span data-ttu-id="778b9-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="778b9-117">Application</span></span>|<span data-ttu-id="778b9-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="778b9-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="778b9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="778b9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformance/{userExperienceAnalyticsAppHealthApplicationPerformanceId}
```

## <a name="request-headers"></a><span data-ttu-id="778b9-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="778b9-120">Request headers</span></span>
|<span data-ttu-id="778b9-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="778b9-121">Header</span></span>|<span data-ttu-id="778b9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="778b9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="778b9-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="778b9-123">Authorization</span></span>|<span data-ttu-id="778b9-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="778b9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="778b9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="778b9-125">Accept</span></span>|<span data-ttu-id="778b9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="778b9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="778b9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="778b9-127">Request body</span></span>
<span data-ttu-id="778b9-128">В тексте запроса добавьте представление объекта [усерекспериенцеаналитиксапфеалсаппликатионперформанце](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="778b9-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) object.</span></span>

<span data-ttu-id="778b9-129">В следующей таблице приведены свойства, необходимые при создании [усерекспериенцеаналитиксапфеалсаппликатионперформанце](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md).</span><span class="sxs-lookup"><span data-stu-id="778b9-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md).</span></span>

|<span data-ttu-id="778b9-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="778b9-130">Property</span></span>|<span data-ttu-id="778b9-131">Тип</span><span class="sxs-lookup"><span data-stu-id="778b9-131">Type</span></span>|<span data-ttu-id="778b9-132">Описание</span><span class="sxs-lookup"><span data-stu-id="778b9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="778b9-133">id</span><span class="sxs-lookup"><span data-stu-id="778b9-133">id</span></span>|<span data-ttu-id="778b9-134">String</span><span class="sxs-lookup"><span data-stu-id="778b9-134">String</span></span>|<span data-ttu-id="778b9-135">Уникальный идентификатор объекта производительности приложения аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="778b9-135">The unique identifier of the user experience analytics app performance object.</span></span>|
|<span data-ttu-id="778b9-136">appName</span><span class="sxs-lookup"><span data-stu-id="778b9-136">appName</span></span>|<span data-ttu-id="778b9-137">String</span><span class="sxs-lookup"><span data-stu-id="778b9-137">String</span></span>|<span data-ttu-id="778b9-138">Имя приложения.</span><span class="sxs-lookup"><span data-stu-id="778b9-138">The name of the application.</span></span>|
|<span data-ttu-id="778b9-139">аппфриендлинаме</span><span class="sxs-lookup"><span data-stu-id="778b9-139">appFriendlyName</span></span>|<span data-ttu-id="778b9-140">String</span><span class="sxs-lookup"><span data-stu-id="778b9-140">String</span></span>|<span data-ttu-id="778b9-141">Понятное имя приложения.</span><span class="sxs-lookup"><span data-stu-id="778b9-141">The friendly name of the application.</span></span>|
|<span data-ttu-id="778b9-142">апппублишер</span><span class="sxs-lookup"><span data-stu-id="778b9-142">appPublisher</span></span>|<span data-ttu-id="778b9-143">String</span><span class="sxs-lookup"><span data-stu-id="778b9-143">String</span></span>|<span data-ttu-id="778b9-144">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="778b9-144">The publisher of the application.</span></span>|
|<span data-ttu-id="778b9-145">активедевицес</span><span class="sxs-lookup"><span data-stu-id="778b9-145">activeDevices</span></span>|<span data-ttu-id="778b9-146">Int32</span><span class="sxs-lookup"><span data-stu-id="778b9-146">Int32</span></span>|<span data-ttu-id="778b9-147">Количество устройств, в которых приложение было активно.</span><span class="sxs-lookup"><span data-stu-id="778b9-147">The number of devices where the app has been active.</span></span> <span data-ttu-id="778b9-148">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="778b9-148">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="778b9-149">тоталаппусажедуратион</span><span class="sxs-lookup"><span data-stu-id="778b9-149">totalAppUsageDuration</span></span>|<span data-ttu-id="778b9-150">Int32</span><span class="sxs-lookup"><span data-stu-id="778b9-150">Int32</span></span>|<span data-ttu-id="778b9-151">Общее время использования приложения в минутах.</span><span class="sxs-lookup"><span data-stu-id="778b9-151">The total usage time of the application in minutes.</span></span> <span data-ttu-id="778b9-152">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="778b9-152">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="778b9-153">тоталаппкрашес</span><span class="sxs-lookup"><span data-stu-id="778b9-153">totalAppCrashes</span></span>|<span data-ttu-id="778b9-154">Int32</span><span class="sxs-lookup"><span data-stu-id="778b9-154">Int32</span></span>|<span data-ttu-id="778b9-155">Число сбоев для приложения.</span><span class="sxs-lookup"><span data-stu-id="778b9-155">The number of crashes for the app.</span></span> <span data-ttu-id="778b9-156">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="778b9-156">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="778b9-157">тоталапфангс</span><span class="sxs-lookup"><span data-stu-id="778b9-157">totalAppHangs</span></span>|<span data-ttu-id="778b9-158">Int32</span><span class="sxs-lookup"><span data-stu-id="778b9-158">Int32</span></span>|<span data-ttu-id="778b9-159">Число зависаний для приложения.</span><span class="sxs-lookup"><span data-stu-id="778b9-159">The number of hangs for the app.</span></span> <span data-ttu-id="778b9-160">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="778b9-160">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="778b9-161">меантиметофаилуре</span><span class="sxs-lookup"><span data-stu-id="778b9-161">meanTimeToFailure</span></span>|<span data-ttu-id="778b9-162">Int32</span><span class="sxs-lookup"><span data-stu-id="778b9-162">Int32</span></span>|<span data-ttu-id="778b9-163">Среднее время до сбоя приложения в минутах.</span><span class="sxs-lookup"><span data-stu-id="778b9-163">The mean time to failure for the app in minutes.</span></span> <span data-ttu-id="778b9-164">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="778b9-164">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="778b9-165">апфеалсскоре</span><span class="sxs-lookup"><span data-stu-id="778b9-165">appHealthScore</span></span>|<span data-ttu-id="778b9-166">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="778b9-166">Double</span></span>|<span data-ttu-id="778b9-167">Оценка работоспособности приложения.</span><span class="sxs-lookup"><span data-stu-id="778b9-167">The health score of the app.</span></span> <span data-ttu-id="778b9-168">Допустимые значения — 1 79769313486232e308 E + 308 — 1 79769313486232e308 E + 308</span><span class="sxs-lookup"><span data-stu-id="778b9-168">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="778b9-169">апфеалсстатус</span><span class="sxs-lookup"><span data-stu-id="778b9-169">appHealthStatus</span></span>|<span data-ttu-id="778b9-170">String</span><span class="sxs-lookup"><span data-stu-id="778b9-170">String</span></span>|<span data-ttu-id="778b9-171">Общее состояние работоспособности приложения.</span><span class="sxs-lookup"><span data-stu-id="778b9-171">The overall health status of the app.</span></span>|
|<span data-ttu-id="778b9-172">аллоргшеалсскоре</span><span class="sxs-lookup"><span data-stu-id="778b9-172">allOrgsHealthScore</span></span>|<span data-ttu-id="778b9-173">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="778b9-173">Double</span></span>|<span data-ttu-id="778b9-174">Медианный показатель работоспособности приложения во всех организациях.</span><span class="sxs-lookup"><span data-stu-id="778b9-174">The median health score of the application across all organizations.</span></span> <span data-ttu-id="778b9-175">Допустимые значения — 1 79769313486232e308 E + 308 — 1 79769313486232e308 E + 308</span><span class="sxs-lookup"><span data-stu-id="778b9-175">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="778b9-176">аллоргсмеантиметофаилуре</span><span class="sxs-lookup"><span data-stu-id="778b9-176">allOrgsMeanTimeToFailure</span></span>|<span data-ttu-id="778b9-177">Int32</span><span class="sxs-lookup"><span data-stu-id="778b9-177">Int32</span></span>|<span data-ttu-id="778b9-178">Среднее время сбоя для всех организаций для приложения в минутах.</span><span class="sxs-lookup"><span data-stu-id="778b9-178">The median mean time to failure across all orgs for the app in minutes.</span></span> <span data-ttu-id="778b9-179">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="778b9-179">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="778b9-180">tenantId</span><span class="sxs-lookup"><span data-stu-id="778b9-180">tenantId</span></span>|<span data-ttu-id="778b9-181">String</span><span class="sxs-lookup"><span data-stu-id="778b9-181">String</span></span>|<span data-ttu-id="778b9-182">Идентификатор клиента, связанного с этим объектом App.</span><span class="sxs-lookup"><span data-stu-id="778b9-182">The id of the tenant associated with this app object.</span></span>|
|<span data-ttu-id="778b9-183">мематимеженератед</span><span class="sxs-lookup"><span data-stu-id="778b9-183">memaTimeGenerated</span></span>|<span data-ttu-id="778b9-184">String</span><span class="sxs-lookup"><span data-stu-id="778b9-184">String</span></span>|<span data-ttu-id="778b9-185">Время, когда агрегация была выполнена в мема.</span><span class="sxs-lookup"><span data-stu-id="778b9-185">The time when aggregation was performed in MEMA.</span></span>|



## <a name="response"></a><span data-ttu-id="778b9-186">Ответ</span><span class="sxs-lookup"><span data-stu-id="778b9-186">Response</span></span>
<span data-ttu-id="778b9-187">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [усерекспериенцеаналитиксапфеалсаппликатионперформанце](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="778b9-187">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="778b9-188">Пример</span><span class="sxs-lookup"><span data-stu-id="778b9-188">Example</span></span>

### <a name="request"></a><span data-ttu-id="778b9-189">Запрос</span><span class="sxs-lookup"><span data-stu-id="778b9-189">Request</span></span>
<span data-ttu-id="778b9-190">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="778b9-190">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformance/{userExperienceAnalyticsAppHealthApplicationPerformanceId}
Content-type: application/json
Content-length: 591

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthApplicationPerformance",
  "appName": "App Name value",
  "appFriendlyName": "App Friendly Name value",
  "appPublisher": "App Publisher value",
  "activeDevices": 13,
  "totalAppUsageDuration": 5,
  "totalAppCrashes": 15,
  "totalAppHangs": 13,
  "meanTimeToFailure": 1,
  "appHealthScore": 4.666666666666667,
  "appHealthStatus": "App Health Status value",
  "allOrgsHealthScore": 6.0,
  "allOrgsMeanTimeToFailure": 8,
  "tenantId": "Tenant Id value",
  "memaTimeGenerated": "Mema Time Generated value"
}
```

### <a name="response"></a><span data-ttu-id="778b9-191">Отклик</span><span class="sxs-lookup"><span data-stu-id="778b9-191">Response</span></span>
<span data-ttu-id="778b9-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="778b9-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 640

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthApplicationPerformance",
  "id": "c7962a87-2a87-c796-872a-96c7872a96c7",
  "appName": "App Name value",
  "appFriendlyName": "App Friendly Name value",
  "appPublisher": "App Publisher value",
  "activeDevices": 13,
  "totalAppUsageDuration": 5,
  "totalAppCrashes": 15,
  "totalAppHangs": 13,
  "meanTimeToFailure": 1,
  "appHealthScore": 4.666666666666667,
  "appHealthStatus": "App Health Status value",
  "allOrgsHealthScore": 6.0,
  "allOrgsMeanTimeToFailure": 8,
  "tenantId": "Tenant Id value",
  "memaTimeGenerated": "Mema Time Generated value"
}
```



