---
title: Создание userExperienceAnalyticsAppHealthApplicationPerformance
description: Создание нового объекта userExperienceAnalyticsAppHealthApplicationPerformance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 88b30b5a640475bf6d137f2464d4caf1296167d0
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51158173"
---
# <a name="create-userexperienceanalyticsapphealthapplicationperformance"></a><span data-ttu-id="661af-103">Создание userExperienceAnalyticsAppHealthApplicationPerformance</span><span class="sxs-lookup"><span data-stu-id="661af-103">Create userExperienceAnalyticsAppHealthApplicationPerformance</span></span>

<span data-ttu-id="661af-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="661af-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="661af-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="661af-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="661af-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="661af-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="661af-107">Создание нового [объекта userExperienceAnalyticsAppHealthApplicationPerformance.](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md)</span><span class="sxs-lookup"><span data-stu-id="661af-107">Create a new [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="661af-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="661af-108">Prerequisites</span></span>
<span data-ttu-id="661af-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="661af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="661af-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="661af-111">Permission type</span></span>|<span data-ttu-id="661af-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="661af-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="661af-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="661af-113">Delegated (work or school account)</span></span>|<span data-ttu-id="661af-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="661af-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="661af-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="661af-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="661af-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="661af-116">Not supported.</span></span>|
|<span data-ttu-id="661af-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="661af-117">Application</span></span>|<span data-ttu-id="661af-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="661af-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="661af-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="661af-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformance
```

## <a name="request-headers"></a><span data-ttu-id="661af-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="661af-120">Request headers</span></span>
|<span data-ttu-id="661af-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="661af-121">Header</span></span>|<span data-ttu-id="661af-122">Значение</span><span class="sxs-lookup"><span data-stu-id="661af-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="661af-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="661af-123">Authorization</span></span>|<span data-ttu-id="661af-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="661af-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="661af-125">Accept</span><span class="sxs-lookup"><span data-stu-id="661af-125">Accept</span></span>|<span data-ttu-id="661af-126">application/json</span><span class="sxs-lookup"><span data-stu-id="661af-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="661af-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="661af-127">Request body</span></span>
<span data-ttu-id="661af-128">В теле запроса поставляем представление JSON для объекта userExperienceAnalyticsAppHealthApplicationPerformance.</span><span class="sxs-lookup"><span data-stu-id="661af-128">In the request body, supply a JSON representation for the userExperienceAnalyticsAppHealthApplicationPerformance object.</span></span>

<span data-ttu-id="661af-129">В следующей таблице показаны свойства, необходимые при создании userExperienceAnalyticsAppHealthApplicationPerformance.</span><span class="sxs-lookup"><span data-stu-id="661af-129">The following table shows the properties that are required when you create the userExperienceAnalyticsAppHealthApplicationPerformance.</span></span>

|<span data-ttu-id="661af-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="661af-130">Property</span></span>|<span data-ttu-id="661af-131">Тип</span><span class="sxs-lookup"><span data-stu-id="661af-131">Type</span></span>|<span data-ttu-id="661af-132">Описание</span><span class="sxs-lookup"><span data-stu-id="661af-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="661af-133">id</span><span class="sxs-lookup"><span data-stu-id="661af-133">id</span></span>|<span data-ttu-id="661af-134">Строка</span><span class="sxs-lookup"><span data-stu-id="661af-134">String</span></span>|<span data-ttu-id="661af-135">Уникальный идентификатор объекта производительности приложения для аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="661af-135">The unique identifier of the user experience analytics app performance object.</span></span>|
|<span data-ttu-id="661af-136">appHangCount</span><span class="sxs-lookup"><span data-stu-id="661af-136">appHangCount</span></span>|<span data-ttu-id="661af-137">Int32</span><span class="sxs-lookup"><span data-stu-id="661af-137">Int32</span></span>|<span data-ttu-id="661af-138">Количество зависает для приложения.</span><span class="sxs-lookup"><span data-stu-id="661af-138">The number of hangs for the app.</span></span> <span data-ttu-id="661af-139">Допустимые значения -2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="661af-139">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="661af-140">appHealthScore</span><span class="sxs-lookup"><span data-stu-id="661af-140">appHealthScore</span></span>|<span data-ttu-id="661af-141">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="661af-141">Double</span></span>|<span data-ttu-id="661af-142">Оценка состояния здоровья приложения.</span><span class="sxs-lookup"><span data-stu-id="661af-142">The health score of the app.</span></span> <span data-ttu-id="661af-143">Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308</span><span class="sxs-lookup"><span data-stu-id="661af-143">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="661af-144">appHealthStatus</span><span class="sxs-lookup"><span data-stu-id="661af-144">appHealthStatus</span></span>|<span data-ttu-id="661af-145">Строка</span><span class="sxs-lookup"><span data-stu-id="661af-145">String</span></span>|<span data-ttu-id="661af-146">Общее состояние здоровья приложения.</span><span class="sxs-lookup"><span data-stu-id="661af-146">The overall health status of the app.</span></span>|
|<span data-ttu-id="661af-147">allOrgsHealthScore</span><span class="sxs-lookup"><span data-stu-id="661af-147">allOrgsHealthScore</span></span>|<span data-ttu-id="661af-148">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="661af-148">Double</span></span>|<span data-ttu-id="661af-149">Медиана оценка состояния здоровья приложения во всех организациях.</span><span class="sxs-lookup"><span data-stu-id="661af-149">The median health score of the application across all organizations.</span></span> <span data-ttu-id="661af-150">Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308</span><span class="sxs-lookup"><span data-stu-id="661af-150">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="661af-151">activeDeviceCount</span><span class="sxs-lookup"><span data-stu-id="661af-151">activeDeviceCount</span></span>|<span data-ttu-id="661af-152">Int32</span><span class="sxs-lookup"><span data-stu-id="661af-152">Int32</span></span>|<span data-ttu-id="661af-153">Количество устройств, на которых приложение было активным.</span><span class="sxs-lookup"><span data-stu-id="661af-153">The number of devices where the app has been active.</span></span> <span data-ttu-id="661af-154">Допустимые значения -2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="661af-154">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="661af-155">appName</span><span class="sxs-lookup"><span data-stu-id="661af-155">appName</span></span>|<span data-ttu-id="661af-156">String</span><span class="sxs-lookup"><span data-stu-id="661af-156">String</span></span>|<span data-ttu-id="661af-157">Имя приложения.</span><span class="sxs-lookup"><span data-stu-id="661af-157">The name of the application.</span></span>|
|<span data-ttu-id="661af-158">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="661af-158">appDisplayName</span></span>|<span data-ttu-id="661af-159">String</span><span class="sxs-lookup"><span data-stu-id="661af-159">String</span></span>|<span data-ttu-id="661af-160">Удобное имя приложения.</span><span class="sxs-lookup"><span data-stu-id="661af-160">The friendly name of the application.</span></span>|
|<span data-ttu-id="661af-161">appPublisher</span><span class="sxs-lookup"><span data-stu-id="661af-161">appPublisher</span></span>|<span data-ttu-id="661af-162">Строка</span><span class="sxs-lookup"><span data-stu-id="661af-162">String</span></span>|<span data-ttu-id="661af-163">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="661af-163">The publisher of the application.</span></span>|
|<span data-ttu-id="661af-164">appUsageDuration</span><span class="sxs-lookup"><span data-stu-id="661af-164">appUsageDuration</span></span>|<span data-ttu-id="661af-165">Int32</span><span class="sxs-lookup"><span data-stu-id="661af-165">Int32</span></span>|<span data-ttu-id="661af-166">Общее время использования приложения в минутах.</span><span class="sxs-lookup"><span data-stu-id="661af-166">The total usage time of the application in minutes.</span></span> <span data-ttu-id="661af-167">Допустимые значения -2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="661af-167">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="661af-168">appCrashCount</span><span class="sxs-lookup"><span data-stu-id="661af-168">appCrashCount</span></span>|<span data-ttu-id="661af-169">Int32</span><span class="sxs-lookup"><span data-stu-id="661af-169">Int32</span></span>|<span data-ttu-id="661af-170">Количество сбоей для приложения.</span><span class="sxs-lookup"><span data-stu-id="661af-170">The number of crashes for the app.</span></span> <span data-ttu-id="661af-171">Допустимые значения -2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="661af-171">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="661af-172">meanTimeToFailureInMinutes</span><span class="sxs-lookup"><span data-stu-id="661af-172">meanTimeToFailureInMinutes</span></span>|<span data-ttu-id="661af-173">Int32</span><span class="sxs-lookup"><span data-stu-id="661af-173">Int32</span></span>|<span data-ttu-id="661af-174">Время сбоя для приложения в минутах.</span><span class="sxs-lookup"><span data-stu-id="661af-174">The mean time to failure for the app in minutes.</span></span> <span data-ttu-id="661af-175">Допустимые значения -2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="661af-175">Valid values -2147483648 to 2147483647</span></span>|



## <a name="response"></a><span data-ttu-id="661af-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="661af-176">Response</span></span>
<span data-ttu-id="661af-177">В случае успеха этот метод возвращает код отклика и `201 Created` [объект userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="661af-177">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="661af-178">Пример</span><span class="sxs-lookup"><span data-stu-id="661af-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="661af-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="661af-179">Request</span></span>
<span data-ttu-id="661af-180">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="661af-180">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="661af-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="661af-181">Response</span></span>
<span data-ttu-id="661af-p109">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="661af-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




