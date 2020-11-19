---
title: Обновление Усерекспериенцеаналитиксапфеалсаппликатионперформанце
description: Обновление свойств объекта Усерекспериенцеаналитиксапфеалсаппликатионперформанце.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e98f70a5c65435feda1bf8bd88ba294905b07526
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49228388"
---
# <a name="update-userexperienceanalyticsapphealthapplicationperformance"></a><span data-ttu-id="3d8b0-103">Обновление Усерекспериенцеаналитиксапфеалсаппликатионперформанце</span><span class="sxs-lookup"><span data-stu-id="3d8b0-103">Update userExperienceAnalyticsAppHealthApplicationPerformance</span></span>

<span data-ttu-id="3d8b0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d8b0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3d8b0-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d8b0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3d8b0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3d8b0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d8b0-107">Обновление свойств объекта [усерекспериенцеаналитиксапфеалсаппликатионперформанце](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) .</span><span class="sxs-lookup"><span data-stu-id="3d8b0-107">Update the properties of a [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3d8b0-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3d8b0-108">Prerequisites</span></span>
<span data-ttu-id="3d8b0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3d8b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d8b0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3d8b0-111">Permission type</span></span>|<span data-ttu-id="3d8b0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3d8b0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3d8b0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3d8b0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3d8b0-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d8b0-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="3d8b0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3d8b0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3d8b0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d8b0-116">Not supported.</span></span>|
|<span data-ttu-id="3d8b0-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="3d8b0-117">Application</span></span>|<span data-ttu-id="3d8b0-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d8b0-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3d8b0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3d8b0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformance/{userExperienceAnalyticsAppHealthApplicationPerformanceId}
```

## <a name="request-headers"></a><span data-ttu-id="3d8b0-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3d8b0-120">Request headers</span></span>
|<span data-ttu-id="3d8b0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3d8b0-121">Header</span></span>|<span data-ttu-id="3d8b0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3d8b0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3d8b0-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3d8b0-123">Authorization</span></span>|<span data-ttu-id="3d8b0-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3d8b0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3d8b0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3d8b0-125">Accept</span></span>|<span data-ttu-id="3d8b0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3d8b0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d8b0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3d8b0-127">Request body</span></span>
<span data-ttu-id="3d8b0-128">В тексте запроса добавьте представление объекта [усерекспериенцеаналитиксапфеалсаппликатионперформанце](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3d8b0-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) object.</span></span>

<span data-ttu-id="3d8b0-129">В следующей таблице приведены свойства, необходимые при создании [усерекспериенцеаналитиксапфеалсаппликатионперформанце](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md).</span><span class="sxs-lookup"><span data-stu-id="3d8b0-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md).</span></span>

|<span data-ttu-id="3d8b0-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3d8b0-130">Property</span></span>|<span data-ttu-id="3d8b0-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3d8b0-131">Type</span></span>|<span data-ttu-id="3d8b0-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3d8b0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d8b0-133">id</span><span class="sxs-lookup"><span data-stu-id="3d8b0-133">id</span></span>|<span data-ttu-id="3d8b0-134">String</span><span class="sxs-lookup"><span data-stu-id="3d8b0-134">String</span></span>|<span data-ttu-id="3d8b0-135">Уникальный идентификатор объекта производительности приложения аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="3d8b0-135">The unique identifier of the user experience analytics app performance object.</span></span>|
|<span data-ttu-id="3d8b0-136">апфангкаунт</span><span class="sxs-lookup"><span data-stu-id="3d8b0-136">appHangCount</span></span>|<span data-ttu-id="3d8b0-137">Int32</span><span class="sxs-lookup"><span data-stu-id="3d8b0-137">Int32</span></span>|<span data-ttu-id="3d8b0-138">Число зависаний для приложения.</span><span class="sxs-lookup"><span data-stu-id="3d8b0-138">The number of hangs for the app.</span></span> <span data-ttu-id="3d8b0-139">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="3d8b0-139">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="3d8b0-140">апфеалсскоре</span><span class="sxs-lookup"><span data-stu-id="3d8b0-140">appHealthScore</span></span>|<span data-ttu-id="3d8b0-141">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="3d8b0-141">Double</span></span>|<span data-ttu-id="3d8b0-142">Оценка работоспособности приложения.</span><span class="sxs-lookup"><span data-stu-id="3d8b0-142">The health score of the app.</span></span> <span data-ttu-id="3d8b0-143">Допустимые значения — 1 79769313486232e308 E + 308 — 1 79769313486232e308 E + 308</span><span class="sxs-lookup"><span data-stu-id="3d8b0-143">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="3d8b0-144">апфеалсстатус</span><span class="sxs-lookup"><span data-stu-id="3d8b0-144">appHealthStatus</span></span>|<span data-ttu-id="3d8b0-145">String</span><span class="sxs-lookup"><span data-stu-id="3d8b0-145">String</span></span>|<span data-ttu-id="3d8b0-146">Общее состояние работоспособности приложения.</span><span class="sxs-lookup"><span data-stu-id="3d8b0-146">The overall health status of the app.</span></span>|
|<span data-ttu-id="3d8b0-147">аллоргшеалсскоре</span><span class="sxs-lookup"><span data-stu-id="3d8b0-147">allOrgsHealthScore</span></span>|<span data-ttu-id="3d8b0-148">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="3d8b0-148">Double</span></span>|<span data-ttu-id="3d8b0-149">Медианный показатель работоспособности приложения во всех организациях.</span><span class="sxs-lookup"><span data-stu-id="3d8b0-149">The median health score of the application across all organizations.</span></span> <span data-ttu-id="3d8b0-150">Допустимые значения — 1 79769313486232e308 E + 308 — 1 79769313486232e308 E + 308</span><span class="sxs-lookup"><span data-stu-id="3d8b0-150">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="3d8b0-151">активедевицекаунт</span><span class="sxs-lookup"><span data-stu-id="3d8b0-151">activeDeviceCount</span></span>|<span data-ttu-id="3d8b0-152">Int32</span><span class="sxs-lookup"><span data-stu-id="3d8b0-152">Int32</span></span>|<span data-ttu-id="3d8b0-153">Количество устройств, в которых приложение было активно.</span><span class="sxs-lookup"><span data-stu-id="3d8b0-153">The number of devices where the app has been active.</span></span> <span data-ttu-id="3d8b0-154">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="3d8b0-154">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="3d8b0-155">appName</span><span class="sxs-lookup"><span data-stu-id="3d8b0-155">appName</span></span>|<span data-ttu-id="3d8b0-156">String</span><span class="sxs-lookup"><span data-stu-id="3d8b0-156">String</span></span>|<span data-ttu-id="3d8b0-157">Имя приложения.</span><span class="sxs-lookup"><span data-stu-id="3d8b0-157">The name of the application.</span></span>|
|<span data-ttu-id="3d8b0-158">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="3d8b0-158">appDisplayName</span></span>|<span data-ttu-id="3d8b0-159">String</span><span class="sxs-lookup"><span data-stu-id="3d8b0-159">String</span></span>|<span data-ttu-id="3d8b0-160">Понятное имя приложения.</span><span class="sxs-lookup"><span data-stu-id="3d8b0-160">The friendly name of the application.</span></span>|
|<span data-ttu-id="3d8b0-161">апппублишер</span><span class="sxs-lookup"><span data-stu-id="3d8b0-161">appPublisher</span></span>|<span data-ttu-id="3d8b0-162">String</span><span class="sxs-lookup"><span data-stu-id="3d8b0-162">String</span></span>|<span data-ttu-id="3d8b0-163">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="3d8b0-163">The publisher of the application.</span></span>|
|<span data-ttu-id="3d8b0-164">аппусажедуратион</span><span class="sxs-lookup"><span data-stu-id="3d8b0-164">appUsageDuration</span></span>|<span data-ttu-id="3d8b0-165">Int32</span><span class="sxs-lookup"><span data-stu-id="3d8b0-165">Int32</span></span>|<span data-ttu-id="3d8b0-166">Общее время использования приложения в минутах.</span><span class="sxs-lookup"><span data-stu-id="3d8b0-166">The total usage time of the application in minutes.</span></span> <span data-ttu-id="3d8b0-167">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="3d8b0-167">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="3d8b0-168">аппкрашкаунт</span><span class="sxs-lookup"><span data-stu-id="3d8b0-168">appCrashCount</span></span>|<span data-ttu-id="3d8b0-169">Int32</span><span class="sxs-lookup"><span data-stu-id="3d8b0-169">Int32</span></span>|<span data-ttu-id="3d8b0-170">Число сбоев для приложения.</span><span class="sxs-lookup"><span data-stu-id="3d8b0-170">The number of crashes for the app.</span></span> <span data-ttu-id="3d8b0-171">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="3d8b0-171">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="3d8b0-172">меантиметофаилуреинминутес</span><span class="sxs-lookup"><span data-stu-id="3d8b0-172">meanTimeToFailureInMinutes</span></span>|<span data-ttu-id="3d8b0-173">Int32</span><span class="sxs-lookup"><span data-stu-id="3d8b0-173">Int32</span></span>|<span data-ttu-id="3d8b0-174">Среднее время до сбоя приложения в минутах.</span><span class="sxs-lookup"><span data-stu-id="3d8b0-174">The mean time to failure for the app in minutes.</span></span> <span data-ttu-id="3d8b0-175">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="3d8b0-175">Valid values -2147483648 to 2147483647</span></span>|



## <a name="response"></a><span data-ttu-id="3d8b0-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="3d8b0-176">Response</span></span>
<span data-ttu-id="3d8b0-177">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [усерекспериенцеаналитиксапфеалсаппликатионперформанце](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3d8b0-177">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d8b0-178">Пример</span><span class="sxs-lookup"><span data-stu-id="3d8b0-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="3d8b0-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="3d8b0-179">Request</span></span>
<span data-ttu-id="3d8b0-180">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3d8b0-180">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3d8b0-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="3d8b0-181">Response</span></span>
<span data-ttu-id="3d8b0-p109">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3d8b0-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




