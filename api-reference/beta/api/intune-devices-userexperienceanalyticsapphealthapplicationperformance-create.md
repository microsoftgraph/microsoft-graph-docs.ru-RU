---
title: Создание Усерекспериенцеаналитиксапфеалсаппликатионперформанце
description: Создание нового объекта Усерекспериенцеаналитиксапфеалсаппликатионперформанце.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3cf8c7485bca42f5d2a776033c70232a87e9411f
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48703176"
---
# <a name="create-userexperienceanalyticsapphealthapplicationperformance"></a><span data-ttu-id="85d90-103">Создание Усерекспериенцеаналитиксапфеалсаппликатионперформанце</span><span class="sxs-lookup"><span data-stu-id="85d90-103">Create userExperienceAnalyticsAppHealthApplicationPerformance</span></span>

<span data-ttu-id="85d90-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85d90-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="85d90-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85d90-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="85d90-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="85d90-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85d90-107">Создание нового объекта [усерекспериенцеаналитиксапфеалсаппликатионперформанце](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) .</span><span class="sxs-lookup"><span data-stu-id="85d90-107">Create a new [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="85d90-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="85d90-108">Prerequisites</span></span>
<span data-ttu-id="85d90-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85d90-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85d90-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="85d90-111">Permission type</span></span>|<span data-ttu-id="85d90-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="85d90-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85d90-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="85d90-113">Delegated (work or school account)</span></span>|<span data-ttu-id="85d90-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85d90-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="85d90-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="85d90-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85d90-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85d90-116">Not supported.</span></span>|
|<span data-ttu-id="85d90-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="85d90-117">Application</span></span>|<span data-ttu-id="85d90-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85d90-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="85d90-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="85d90-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformance
```

## <a name="request-headers"></a><span data-ttu-id="85d90-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="85d90-120">Request headers</span></span>
|<span data-ttu-id="85d90-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="85d90-121">Header</span></span>|<span data-ttu-id="85d90-122">Значение</span><span class="sxs-lookup"><span data-stu-id="85d90-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="85d90-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="85d90-123">Authorization</span></span>|<span data-ttu-id="85d90-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="85d90-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="85d90-125">Accept</span><span class="sxs-lookup"><span data-stu-id="85d90-125">Accept</span></span>|<span data-ttu-id="85d90-126">application/json</span><span class="sxs-lookup"><span data-stu-id="85d90-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="85d90-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="85d90-127">Request body</span></span>
<span data-ttu-id="85d90-128">В тексте запроса добавьте представление объекта Усерекспериенцеаналитиксапфеалсаппликатионперформанце в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="85d90-128">In the request body, supply a JSON representation for the userExperienceAnalyticsAppHealthApplicationPerformance object.</span></span>

<span data-ttu-id="85d90-129">В следующей таблице приведены свойства, необходимые при создании Усерекспериенцеаналитиксапфеалсаппликатионперформанце.</span><span class="sxs-lookup"><span data-stu-id="85d90-129">The following table shows the properties that are required when you create the userExperienceAnalyticsAppHealthApplicationPerformance.</span></span>

|<span data-ttu-id="85d90-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="85d90-130">Property</span></span>|<span data-ttu-id="85d90-131">Тип</span><span class="sxs-lookup"><span data-stu-id="85d90-131">Type</span></span>|<span data-ttu-id="85d90-132">Описание</span><span class="sxs-lookup"><span data-stu-id="85d90-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85d90-133">id</span><span class="sxs-lookup"><span data-stu-id="85d90-133">id</span></span>|<span data-ttu-id="85d90-134">Строка</span><span class="sxs-lookup"><span data-stu-id="85d90-134">String</span></span>|<span data-ttu-id="85d90-135">Уникальный идентификатор объекта производительности приложения аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="85d90-135">The unique identifier of the user experience analytics app performance object.</span></span>|
|<span data-ttu-id="85d90-136">апфангкаунт</span><span class="sxs-lookup"><span data-stu-id="85d90-136">appHangCount</span></span>|<span data-ttu-id="85d90-137">Int32</span><span class="sxs-lookup"><span data-stu-id="85d90-137">Int32</span></span>|<span data-ttu-id="85d90-138">Число зависаний для приложения.</span><span class="sxs-lookup"><span data-stu-id="85d90-138">The number of hangs for the app.</span></span> <span data-ttu-id="85d90-139">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="85d90-139">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="85d90-140">апфеалсскоре</span><span class="sxs-lookup"><span data-stu-id="85d90-140">appHealthScore</span></span>|<span data-ttu-id="85d90-141">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="85d90-141">Double</span></span>|<span data-ttu-id="85d90-142">Оценка работоспособности приложения.</span><span class="sxs-lookup"><span data-stu-id="85d90-142">The health score of the app.</span></span> <span data-ttu-id="85d90-143">Допустимые значения — 1 79769313486232e308 E + 308 — 1 79769313486232e308 E + 308</span><span class="sxs-lookup"><span data-stu-id="85d90-143">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="85d90-144">апфеалсстатус</span><span class="sxs-lookup"><span data-stu-id="85d90-144">appHealthStatus</span></span>|<span data-ttu-id="85d90-145">Строка</span><span class="sxs-lookup"><span data-stu-id="85d90-145">String</span></span>|<span data-ttu-id="85d90-146">Общее состояние работоспособности приложения.</span><span class="sxs-lookup"><span data-stu-id="85d90-146">The overall health status of the app.</span></span>|
|<span data-ttu-id="85d90-147">аллоргшеалсскоре</span><span class="sxs-lookup"><span data-stu-id="85d90-147">allOrgsHealthScore</span></span>|<span data-ttu-id="85d90-148">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="85d90-148">Double</span></span>|<span data-ttu-id="85d90-149">Медианный показатель работоспособности приложения во всех организациях.</span><span class="sxs-lookup"><span data-stu-id="85d90-149">The median health score of the application across all organizations.</span></span> <span data-ttu-id="85d90-150">Допустимые значения — 1 79769313486232e308 E + 308 — 1 79769313486232e308 E + 308</span><span class="sxs-lookup"><span data-stu-id="85d90-150">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="85d90-151">активедевицекаунт</span><span class="sxs-lookup"><span data-stu-id="85d90-151">activeDeviceCount</span></span>|<span data-ttu-id="85d90-152">Int32</span><span class="sxs-lookup"><span data-stu-id="85d90-152">Int32</span></span>|<span data-ttu-id="85d90-153">Количество устройств, в которых приложение было активно.</span><span class="sxs-lookup"><span data-stu-id="85d90-153">The number of devices where the app has been active.</span></span> <span data-ttu-id="85d90-154">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="85d90-154">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="85d90-155">appName</span><span class="sxs-lookup"><span data-stu-id="85d90-155">appName</span></span>|<span data-ttu-id="85d90-156">String</span><span class="sxs-lookup"><span data-stu-id="85d90-156">String</span></span>|<span data-ttu-id="85d90-157">Имя приложения.</span><span class="sxs-lookup"><span data-stu-id="85d90-157">The name of the application.</span></span>|
|<span data-ttu-id="85d90-158">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="85d90-158">appDisplayName</span></span>|<span data-ttu-id="85d90-159">String</span><span class="sxs-lookup"><span data-stu-id="85d90-159">String</span></span>|<span data-ttu-id="85d90-160">Понятное имя приложения.</span><span class="sxs-lookup"><span data-stu-id="85d90-160">The friendly name of the application.</span></span>|
|<span data-ttu-id="85d90-161">апппублишер</span><span class="sxs-lookup"><span data-stu-id="85d90-161">appPublisher</span></span>|<span data-ttu-id="85d90-162">Строка</span><span class="sxs-lookup"><span data-stu-id="85d90-162">String</span></span>|<span data-ttu-id="85d90-163">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="85d90-163">The publisher of the application.</span></span>|
|<span data-ttu-id="85d90-164">аппусажедуратион</span><span class="sxs-lookup"><span data-stu-id="85d90-164">appUsageDuration</span></span>|<span data-ttu-id="85d90-165">Int32</span><span class="sxs-lookup"><span data-stu-id="85d90-165">Int32</span></span>|<span data-ttu-id="85d90-166">Общее время использования приложения в минутах.</span><span class="sxs-lookup"><span data-stu-id="85d90-166">The total usage time of the application in minutes.</span></span> <span data-ttu-id="85d90-167">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="85d90-167">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="85d90-168">аппкрашкаунт</span><span class="sxs-lookup"><span data-stu-id="85d90-168">appCrashCount</span></span>|<span data-ttu-id="85d90-169">Int32</span><span class="sxs-lookup"><span data-stu-id="85d90-169">Int32</span></span>|<span data-ttu-id="85d90-170">Число сбоев для приложения.</span><span class="sxs-lookup"><span data-stu-id="85d90-170">The number of crashes for the app.</span></span> <span data-ttu-id="85d90-171">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="85d90-171">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="85d90-172">меантиметофаилуреинминутес</span><span class="sxs-lookup"><span data-stu-id="85d90-172">meanTimeToFailureInMinutes</span></span>|<span data-ttu-id="85d90-173">Int32</span><span class="sxs-lookup"><span data-stu-id="85d90-173">Int32</span></span>|<span data-ttu-id="85d90-174">Среднее время до сбоя приложения в минутах.</span><span class="sxs-lookup"><span data-stu-id="85d90-174">The mean time to failure for the app in minutes.</span></span> <span data-ttu-id="85d90-175">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="85d90-175">Valid values -2147483648 to 2147483647</span></span>|



## <a name="response"></a><span data-ttu-id="85d90-176">Ответ</span><span class="sxs-lookup"><span data-stu-id="85d90-176">Response</span></span>
<span data-ttu-id="85d90-177">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [усерекспериенцеаналитиксапфеалсаппликатионперформанце](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="85d90-177">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85d90-178">Пример</span><span class="sxs-lookup"><span data-stu-id="85d90-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="85d90-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="85d90-179">Request</span></span>
<span data-ttu-id="85d90-180">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="85d90-180">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="85d90-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="85d90-181">Response</span></span>
<span data-ttu-id="85d90-p109">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="85d90-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





