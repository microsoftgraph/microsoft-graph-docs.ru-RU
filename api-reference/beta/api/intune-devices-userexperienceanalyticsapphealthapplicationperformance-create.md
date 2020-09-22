---
title: Создание Усерекспериенцеаналитиксапфеалсаппликатионперформанце
description: Создание нового объекта Усерекспериенцеаналитиксапфеалсаппликатионперформанце.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: aa6818622e9ea0f11c480d7045f6e440c706abca
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48017600"
---
# <a name="create-userexperienceanalyticsapphealthapplicationperformance"></a><span data-ttu-id="74788-103">Создание Усерекспериенцеаналитиксапфеалсаппликатионперформанце</span><span class="sxs-lookup"><span data-stu-id="74788-103">Create userExperienceAnalyticsAppHealthApplicationPerformance</span></span>

<span data-ttu-id="74788-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74788-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="74788-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74788-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="74788-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="74788-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="74788-107">Создание нового объекта [усерекспериенцеаналитиксапфеалсаппликатионперформанце](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) .</span><span class="sxs-lookup"><span data-stu-id="74788-107">Create a new [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="74788-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="74788-108">Prerequisites</span></span>
<span data-ttu-id="74788-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74788-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74788-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="74788-111">Permission type</span></span>|<span data-ttu-id="74788-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="74788-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="74788-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="74788-113">Delegated (work or school account)</span></span>|<span data-ttu-id="74788-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74788-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="74788-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="74788-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="74788-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74788-116">Not supported.</span></span>|
|<span data-ttu-id="74788-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="74788-117">Application</span></span>|<span data-ttu-id="74788-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74788-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="74788-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="74788-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformance
```

## <a name="request-headers"></a><span data-ttu-id="74788-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="74788-120">Request headers</span></span>
|<span data-ttu-id="74788-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="74788-121">Header</span></span>|<span data-ttu-id="74788-122">Значение</span><span class="sxs-lookup"><span data-stu-id="74788-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="74788-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="74788-123">Authorization</span></span>|<span data-ttu-id="74788-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="74788-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="74788-125">Accept</span><span class="sxs-lookup"><span data-stu-id="74788-125">Accept</span></span>|<span data-ttu-id="74788-126">application/json</span><span class="sxs-lookup"><span data-stu-id="74788-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="74788-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="74788-127">Request body</span></span>
<span data-ttu-id="74788-128">В тексте запроса добавьте представление объекта Усерекспериенцеаналитиксапфеалсаппликатионперформанце в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="74788-128">In the request body, supply a JSON representation for the userExperienceAnalyticsAppHealthApplicationPerformance object.</span></span>

<span data-ttu-id="74788-129">В следующей таблице приведены свойства, необходимые при создании Усерекспериенцеаналитиксапфеалсаппликатионперформанце.</span><span class="sxs-lookup"><span data-stu-id="74788-129">The following table shows the properties that are required when you create the userExperienceAnalyticsAppHealthApplicationPerformance.</span></span>

|<span data-ttu-id="74788-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="74788-130">Property</span></span>|<span data-ttu-id="74788-131">Тип</span><span class="sxs-lookup"><span data-stu-id="74788-131">Type</span></span>|<span data-ttu-id="74788-132">Описание</span><span class="sxs-lookup"><span data-stu-id="74788-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74788-133">id</span><span class="sxs-lookup"><span data-stu-id="74788-133">id</span></span>|<span data-ttu-id="74788-134">String</span><span class="sxs-lookup"><span data-stu-id="74788-134">String</span></span>|<span data-ttu-id="74788-135">Уникальный идентификатор объекта производительности приложения аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="74788-135">The unique identifier of the user experience analytics app performance object.</span></span>|
|<span data-ttu-id="74788-136">апфангкаунт</span><span class="sxs-lookup"><span data-stu-id="74788-136">appHangCount</span></span>|<span data-ttu-id="74788-137">Int32</span><span class="sxs-lookup"><span data-stu-id="74788-137">Int32</span></span>|<span data-ttu-id="74788-138">Число зависаний для приложения.</span><span class="sxs-lookup"><span data-stu-id="74788-138">The number of hangs for the app.</span></span> <span data-ttu-id="74788-139">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="74788-139">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="74788-140">апфеалсскоре</span><span class="sxs-lookup"><span data-stu-id="74788-140">appHealthScore</span></span>|<span data-ttu-id="74788-141">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="74788-141">Double</span></span>|<span data-ttu-id="74788-142">Оценка работоспособности приложения.</span><span class="sxs-lookup"><span data-stu-id="74788-142">The health score of the app.</span></span> <span data-ttu-id="74788-143">Допустимые значения — 1 79769313486232e308 E + 308 — 1 79769313486232e308 E + 308</span><span class="sxs-lookup"><span data-stu-id="74788-143">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="74788-144">апфеалсстатус</span><span class="sxs-lookup"><span data-stu-id="74788-144">appHealthStatus</span></span>|<span data-ttu-id="74788-145">String</span><span class="sxs-lookup"><span data-stu-id="74788-145">String</span></span>|<span data-ttu-id="74788-146">Общее состояние работоспособности приложения.</span><span class="sxs-lookup"><span data-stu-id="74788-146">The overall health status of the app.</span></span>|
|<span data-ttu-id="74788-147">аллоргшеалсскоре</span><span class="sxs-lookup"><span data-stu-id="74788-147">allOrgsHealthScore</span></span>|<span data-ttu-id="74788-148">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="74788-148">Double</span></span>|<span data-ttu-id="74788-149">Медианный показатель работоспособности приложения во всех организациях.</span><span class="sxs-lookup"><span data-stu-id="74788-149">The median health score of the application across all organizations.</span></span> <span data-ttu-id="74788-150">Допустимые значения — 1 79769313486232e308 E + 308 — 1 79769313486232e308 E + 308</span><span class="sxs-lookup"><span data-stu-id="74788-150">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="74788-151">активедевицекаунт</span><span class="sxs-lookup"><span data-stu-id="74788-151">activeDeviceCount</span></span>|<span data-ttu-id="74788-152">Int32</span><span class="sxs-lookup"><span data-stu-id="74788-152">Int32</span></span>|<span data-ttu-id="74788-153">Количество устройств, в которых приложение было активно.</span><span class="sxs-lookup"><span data-stu-id="74788-153">The number of devices where the app has been active.</span></span> <span data-ttu-id="74788-154">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="74788-154">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="74788-155">appName</span><span class="sxs-lookup"><span data-stu-id="74788-155">appName</span></span>|<span data-ttu-id="74788-156">String</span><span class="sxs-lookup"><span data-stu-id="74788-156">String</span></span>|<span data-ttu-id="74788-157">Имя приложения.</span><span class="sxs-lookup"><span data-stu-id="74788-157">The name of the application.</span></span>|
|<span data-ttu-id="74788-158">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="74788-158">appDisplayName</span></span>|<span data-ttu-id="74788-159">String</span><span class="sxs-lookup"><span data-stu-id="74788-159">String</span></span>|<span data-ttu-id="74788-160">Понятное имя приложения.</span><span class="sxs-lookup"><span data-stu-id="74788-160">The friendly name of the application.</span></span>|
|<span data-ttu-id="74788-161">апппублишер</span><span class="sxs-lookup"><span data-stu-id="74788-161">appPublisher</span></span>|<span data-ttu-id="74788-162">String</span><span class="sxs-lookup"><span data-stu-id="74788-162">String</span></span>|<span data-ttu-id="74788-163">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="74788-163">The publisher of the application.</span></span>|
|<span data-ttu-id="74788-164">аппусажедуратион</span><span class="sxs-lookup"><span data-stu-id="74788-164">appUsageDuration</span></span>|<span data-ttu-id="74788-165">Int32</span><span class="sxs-lookup"><span data-stu-id="74788-165">Int32</span></span>|<span data-ttu-id="74788-166">Общее время использования приложения в минутах.</span><span class="sxs-lookup"><span data-stu-id="74788-166">The total usage time of the application in minutes.</span></span> <span data-ttu-id="74788-167">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="74788-167">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="74788-168">аппкрашкаунт</span><span class="sxs-lookup"><span data-stu-id="74788-168">appCrashCount</span></span>|<span data-ttu-id="74788-169">Int32</span><span class="sxs-lookup"><span data-stu-id="74788-169">Int32</span></span>|<span data-ttu-id="74788-170">Число сбоев для приложения.</span><span class="sxs-lookup"><span data-stu-id="74788-170">The number of crashes for the app.</span></span> <span data-ttu-id="74788-171">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="74788-171">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="74788-172">меантиметофаилуреинминутес</span><span class="sxs-lookup"><span data-stu-id="74788-172">meanTimeToFailureInMinutes</span></span>|<span data-ttu-id="74788-173">Int32</span><span class="sxs-lookup"><span data-stu-id="74788-173">Int32</span></span>|<span data-ttu-id="74788-174">Среднее время до сбоя приложения в минутах.</span><span class="sxs-lookup"><span data-stu-id="74788-174">The mean time to failure for the app in minutes.</span></span> <span data-ttu-id="74788-175">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="74788-175">Valid values -2147483648 to 2147483647</span></span>|



## <a name="response"></a><span data-ttu-id="74788-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="74788-176">Response</span></span>
<span data-ttu-id="74788-177">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [усерекспериенцеаналитиксапфеалсаппликатионперформанце](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="74788-177">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74788-178">Пример</span><span class="sxs-lookup"><span data-stu-id="74788-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="74788-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="74788-179">Request</span></span>
<span data-ttu-id="74788-180">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="74788-180">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformance
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

### <a name="response"></a><span data-ttu-id="74788-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="74788-181">Response</span></span>
<span data-ttu-id="74788-p109">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="74788-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






