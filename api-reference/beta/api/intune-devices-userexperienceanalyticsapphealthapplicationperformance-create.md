---
title: Создание Усерекспериенцеаналитиксапфеалсаппликатионперформанце
description: Создание нового объекта Усерекспериенцеаналитиксапфеалсаппликатионперформанце.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a25af7c70c5988ad040a827f37fdec92c497223f
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/18/2020
ms.locfileid: "46790306"
---
# <a name="create-userexperienceanalyticsapphealthapplicationperformance"></a><span data-ttu-id="7c9c0-103">Создание Усерекспериенцеаналитиксапфеалсаппликатионперформанце</span><span class="sxs-lookup"><span data-stu-id="7c9c0-103">Create userExperienceAnalyticsAppHealthApplicationPerformance</span></span>

<span data-ttu-id="7c9c0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c9c0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7c9c0-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c9c0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7c9c0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7c9c0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c9c0-107">Создание нового объекта [усерекспериенцеаналитиксапфеалсаппликатионперформанце](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) .</span><span class="sxs-lookup"><span data-stu-id="7c9c0-107">Create a new [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7c9c0-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7c9c0-108">Prerequisites</span></span>
<span data-ttu-id="7c9c0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c9c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c9c0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7c9c0-111">Permission type</span></span>|<span data-ttu-id="7c9c0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7c9c0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c9c0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7c9c0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7c9c0-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c9c0-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="7c9c0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7c9c0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c9c0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c9c0-116">Not supported.</span></span>|
|<span data-ttu-id="7c9c0-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="7c9c0-117">Application</span></span>|<span data-ttu-id="7c9c0-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c9c0-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c9c0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7c9c0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformance
```

## <a name="request-headers"></a><span data-ttu-id="7c9c0-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7c9c0-120">Request headers</span></span>
|<span data-ttu-id="7c9c0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7c9c0-121">Header</span></span>|<span data-ttu-id="7c9c0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7c9c0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c9c0-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7c9c0-123">Authorization</span></span>|<span data-ttu-id="7c9c0-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7c9c0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7c9c0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7c9c0-125">Accept</span></span>|<span data-ttu-id="7c9c0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7c9c0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c9c0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7c9c0-127">Request body</span></span>
<span data-ttu-id="7c9c0-128">В тексте запроса добавьте представление объекта Усерекспериенцеаналитиксапфеалсаппликатионперформанце в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7c9c0-128">In the request body, supply a JSON representation for the userExperienceAnalyticsAppHealthApplicationPerformance object.</span></span>

<span data-ttu-id="7c9c0-129">В следующей таблице приведены свойства, необходимые при создании Усерекспериенцеаналитиксапфеалсаппликатионперформанце.</span><span class="sxs-lookup"><span data-stu-id="7c9c0-129">The following table shows the properties that are required when you create the userExperienceAnalyticsAppHealthApplicationPerformance.</span></span>

|<span data-ttu-id="7c9c0-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7c9c0-130">Property</span></span>|<span data-ttu-id="7c9c0-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7c9c0-131">Type</span></span>|<span data-ttu-id="7c9c0-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7c9c0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c9c0-133">id</span><span class="sxs-lookup"><span data-stu-id="7c9c0-133">id</span></span>|<span data-ttu-id="7c9c0-134">String</span><span class="sxs-lookup"><span data-stu-id="7c9c0-134">String</span></span>|<span data-ttu-id="7c9c0-135">Уникальный идентификатор объекта производительности приложения аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="7c9c0-135">The unique identifier of the user experience analytics app performance object.</span></span>|
|<span data-ttu-id="7c9c0-136">appName</span><span class="sxs-lookup"><span data-stu-id="7c9c0-136">appName</span></span>|<span data-ttu-id="7c9c0-137">String</span><span class="sxs-lookup"><span data-stu-id="7c9c0-137">String</span></span>|<span data-ttu-id="7c9c0-138">Имя приложения.</span><span class="sxs-lookup"><span data-stu-id="7c9c0-138">The name of the application.</span></span>|
|<span data-ttu-id="7c9c0-139">аппфриендлинаме</span><span class="sxs-lookup"><span data-stu-id="7c9c0-139">appFriendlyName</span></span>|<span data-ttu-id="7c9c0-140">String</span><span class="sxs-lookup"><span data-stu-id="7c9c0-140">String</span></span>|<span data-ttu-id="7c9c0-141">Понятное имя приложения.</span><span class="sxs-lookup"><span data-stu-id="7c9c0-141">The friendly name of the application.</span></span>|
|<span data-ttu-id="7c9c0-142">апппублишер</span><span class="sxs-lookup"><span data-stu-id="7c9c0-142">appPublisher</span></span>|<span data-ttu-id="7c9c0-143">String</span><span class="sxs-lookup"><span data-stu-id="7c9c0-143">String</span></span>|<span data-ttu-id="7c9c0-144">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="7c9c0-144">The publisher of the application.</span></span>|
|<span data-ttu-id="7c9c0-145">активедевицес</span><span class="sxs-lookup"><span data-stu-id="7c9c0-145">activeDevices</span></span>|<span data-ttu-id="7c9c0-146">Int32</span><span class="sxs-lookup"><span data-stu-id="7c9c0-146">Int32</span></span>|<span data-ttu-id="7c9c0-147">Количество устройств, в которых приложение было активно.</span><span class="sxs-lookup"><span data-stu-id="7c9c0-147">The number of devices where the app has been active.</span></span> <span data-ttu-id="7c9c0-148">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="7c9c0-148">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="7c9c0-149">тоталаппусажедуратион</span><span class="sxs-lookup"><span data-stu-id="7c9c0-149">totalAppUsageDuration</span></span>|<span data-ttu-id="7c9c0-150">Int32</span><span class="sxs-lookup"><span data-stu-id="7c9c0-150">Int32</span></span>|<span data-ttu-id="7c9c0-151">Общее время использования приложения в минутах.</span><span class="sxs-lookup"><span data-stu-id="7c9c0-151">The total usage time of the application in minutes.</span></span> <span data-ttu-id="7c9c0-152">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="7c9c0-152">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="7c9c0-153">тоталаппкрашес</span><span class="sxs-lookup"><span data-stu-id="7c9c0-153">totalAppCrashes</span></span>|<span data-ttu-id="7c9c0-154">Int32</span><span class="sxs-lookup"><span data-stu-id="7c9c0-154">Int32</span></span>|<span data-ttu-id="7c9c0-155">Число сбоев для приложения.</span><span class="sxs-lookup"><span data-stu-id="7c9c0-155">The number of crashes for the app.</span></span> <span data-ttu-id="7c9c0-156">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="7c9c0-156">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="7c9c0-157">тоталапфангс</span><span class="sxs-lookup"><span data-stu-id="7c9c0-157">totalAppHangs</span></span>|<span data-ttu-id="7c9c0-158">Int32</span><span class="sxs-lookup"><span data-stu-id="7c9c0-158">Int32</span></span>|<span data-ttu-id="7c9c0-159">Число зависаний для приложения.</span><span class="sxs-lookup"><span data-stu-id="7c9c0-159">The number of hangs for the app.</span></span> <span data-ttu-id="7c9c0-160">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="7c9c0-160">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="7c9c0-161">меантиметофаилуре</span><span class="sxs-lookup"><span data-stu-id="7c9c0-161">meanTimeToFailure</span></span>|<span data-ttu-id="7c9c0-162">Int32</span><span class="sxs-lookup"><span data-stu-id="7c9c0-162">Int32</span></span>|<span data-ttu-id="7c9c0-163">Среднее время до сбоя приложения в минутах.</span><span class="sxs-lookup"><span data-stu-id="7c9c0-163">The mean time to failure for the app in minutes.</span></span> <span data-ttu-id="7c9c0-164">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="7c9c0-164">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="7c9c0-165">апфеалсскоре</span><span class="sxs-lookup"><span data-stu-id="7c9c0-165">appHealthScore</span></span>|<span data-ttu-id="7c9c0-166">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="7c9c0-166">Double</span></span>|<span data-ttu-id="7c9c0-167">Оценка работоспособности приложения.</span><span class="sxs-lookup"><span data-stu-id="7c9c0-167">The health score of the app.</span></span> <span data-ttu-id="7c9c0-168">Допустимые значения — 1 79769313486232e308 E + 308 — 1 79769313486232e308 E + 308</span><span class="sxs-lookup"><span data-stu-id="7c9c0-168">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="7c9c0-169">апфеалсстатус</span><span class="sxs-lookup"><span data-stu-id="7c9c0-169">appHealthStatus</span></span>|<span data-ttu-id="7c9c0-170">String</span><span class="sxs-lookup"><span data-stu-id="7c9c0-170">String</span></span>|<span data-ttu-id="7c9c0-171">Общее состояние работоспособности приложения.</span><span class="sxs-lookup"><span data-stu-id="7c9c0-171">The overall health status of the app.</span></span>|
|<span data-ttu-id="7c9c0-172">аллоргшеалсскоре</span><span class="sxs-lookup"><span data-stu-id="7c9c0-172">allOrgsHealthScore</span></span>|<span data-ttu-id="7c9c0-173">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="7c9c0-173">Double</span></span>|<span data-ttu-id="7c9c0-174">Медианный показатель работоспособности приложения во всех организациях.</span><span class="sxs-lookup"><span data-stu-id="7c9c0-174">The median health score of the application across all organizations.</span></span> <span data-ttu-id="7c9c0-175">Допустимые значения — 1 79769313486232e308 E + 308 — 1 79769313486232e308 E + 308</span><span class="sxs-lookup"><span data-stu-id="7c9c0-175">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="7c9c0-176">аллоргсмеантиметофаилуре</span><span class="sxs-lookup"><span data-stu-id="7c9c0-176">allOrgsMeanTimeToFailure</span></span>|<span data-ttu-id="7c9c0-177">Int32</span><span class="sxs-lookup"><span data-stu-id="7c9c0-177">Int32</span></span>|<span data-ttu-id="7c9c0-178">Среднее время сбоя для всех организаций для приложения в минутах.</span><span class="sxs-lookup"><span data-stu-id="7c9c0-178">The median mean time to failure across all orgs for the app in minutes.</span></span> <span data-ttu-id="7c9c0-179">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="7c9c0-179">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="7c9c0-180">tenantId</span><span class="sxs-lookup"><span data-stu-id="7c9c0-180">tenantId</span></span>|<span data-ttu-id="7c9c0-181">String</span><span class="sxs-lookup"><span data-stu-id="7c9c0-181">String</span></span>|<span data-ttu-id="7c9c0-182">Идентификатор клиента, связанного с этим объектом App.</span><span class="sxs-lookup"><span data-stu-id="7c9c0-182">The id of the tenant associated with this app object.</span></span>|
|<span data-ttu-id="7c9c0-183">мематимеженератед</span><span class="sxs-lookup"><span data-stu-id="7c9c0-183">memaTimeGenerated</span></span>|<span data-ttu-id="7c9c0-184">String</span><span class="sxs-lookup"><span data-stu-id="7c9c0-184">String</span></span>|<span data-ttu-id="7c9c0-185">Время, когда агрегация была выполнена в мема.</span><span class="sxs-lookup"><span data-stu-id="7c9c0-185">The time when aggregation was performed in MEMA.</span></span>|



## <a name="response"></a><span data-ttu-id="7c9c0-186">Ответ</span><span class="sxs-lookup"><span data-stu-id="7c9c0-186">Response</span></span>
<span data-ttu-id="7c9c0-187">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [усерекспериенцеаналитиксапфеалсаппликатионперформанце](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7c9c0-187">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c9c0-188">Пример</span><span class="sxs-lookup"><span data-stu-id="7c9c0-188">Example</span></span>

### <a name="request"></a><span data-ttu-id="7c9c0-189">Запрос</span><span class="sxs-lookup"><span data-stu-id="7c9c0-189">Request</span></span>
<span data-ttu-id="7c9c0-190">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7c9c0-190">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformance
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

### <a name="response"></a><span data-ttu-id="7c9c0-191">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c9c0-191">Response</span></span>
<span data-ttu-id="7c9c0-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7c9c0-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



