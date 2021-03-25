---
title: Создание userExperienceAnalyticsAppHealthAppPerformanceByOSVersion
description: Создание нового объекта userExperienceAnalyticsAppHealthAppPerformanceByOSVersion.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4e90ced56c6831005d9d878bcec6ab613e8060c8
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51158033"
---
# <a name="create-userexperienceanalyticsapphealthappperformancebyosversion"></a><span data-ttu-id="1cb8e-103">Создание userExperienceAnalyticsAppHealthAppPerformanceByOSVersion</span><span class="sxs-lookup"><span data-stu-id="1cb8e-103">Create userExperienceAnalyticsAppHealthAppPerformanceByOSVersion</span></span>

<span data-ttu-id="1cb8e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1cb8e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1cb8e-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1cb8e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1cb8e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1cb8e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1cb8e-107">Создание нового [объекта userExperienceAnalyticsAppHealthAppPerformanceByOSVersion.](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md)</span><span class="sxs-lookup"><span data-stu-id="1cb8e-107">Create a new [userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1cb8e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1cb8e-108">Prerequisites</span></span>
<span data-ttu-id="1cb8e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1cb8e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1cb8e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1cb8e-111">Permission type</span></span>|<span data-ttu-id="1cb8e-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1cb8e-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1cb8e-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1cb8e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1cb8e-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1cb8e-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="1cb8e-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1cb8e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1cb8e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1cb8e-116">Not supported.</span></span>|
|<span data-ttu-id="1cb8e-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="1cb8e-117">Application</span></span>|<span data-ttu-id="1cb8e-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1cb8e-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1cb8e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1cb8e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformanceByOSVersion
```

## <a name="request-headers"></a><span data-ttu-id="1cb8e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1cb8e-120">Request headers</span></span>
|<span data-ttu-id="1cb8e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1cb8e-121">Header</span></span>|<span data-ttu-id="1cb8e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1cb8e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1cb8e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1cb8e-123">Authorization</span></span>|<span data-ttu-id="1cb8e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1cb8e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1cb8e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1cb8e-125">Accept</span></span>|<span data-ttu-id="1cb8e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1cb8e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1cb8e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1cb8e-127">Request body</span></span>
<span data-ttu-id="1cb8e-128">В теле запроса поставляем представление JSON для объекта userExperienceAnalyticsAppHealthAppPerformanceByOSVersion.</span><span class="sxs-lookup"><span data-stu-id="1cb8e-128">In the request body, supply a JSON representation for the userExperienceAnalyticsAppHealthAppPerformanceByOSVersion object.</span></span>

<span data-ttu-id="1cb8e-129">В следующей таблице показаны свойства, необходимые при создании userExperienceAnalyticsAppHealthAppPerformanceByOSVersion.</span><span class="sxs-lookup"><span data-stu-id="1cb8e-129">The following table shows the properties that are required when you create the userExperienceAnalyticsAppHealthAppPerformanceByOSVersion.</span></span>

|<span data-ttu-id="1cb8e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1cb8e-130">Property</span></span>|<span data-ttu-id="1cb8e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1cb8e-131">Type</span></span>|<span data-ttu-id="1cb8e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1cb8e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1cb8e-133">id</span><span class="sxs-lookup"><span data-stu-id="1cb8e-133">id</span></span>|<span data-ttu-id="1cb8e-134">Строка</span><span class="sxs-lookup"><span data-stu-id="1cb8e-134">String</span></span>|<span data-ttu-id="1cb8e-135">Уникальный идентификатор объекта производительности версии версии пользовательского интерфейса для аналитики приложений.</span><span class="sxs-lookup"><span data-stu-id="1cb8e-135">The unique identifier of the user experience analytics app version performance object.</span></span>|
|<span data-ttu-id="1cb8e-136">osVersion</span><span class="sxs-lookup"><span data-stu-id="1cb8e-136">osVersion</span></span>|<span data-ttu-id="1cb8e-137">String</span><span class="sxs-lookup"><span data-stu-id="1cb8e-137">String</span></span>|<span data-ttu-id="1cb8e-138">Версия ос приложения.</span><span class="sxs-lookup"><span data-stu-id="1cb8e-138">The os version of the application.</span></span>|
|<span data-ttu-id="1cb8e-139">osBuildNumber</span><span class="sxs-lookup"><span data-stu-id="1cb8e-139">osBuildNumber</span></span>|<span data-ttu-id="1cb8e-140">Строка</span><span class="sxs-lookup"><span data-stu-id="1cb8e-140">String</span></span>|<span data-ttu-id="1cb8e-141">Число сборки ос приложения.</span><span class="sxs-lookup"><span data-stu-id="1cb8e-141">The os build number of the application.</span></span>|
|<span data-ttu-id="1cb8e-142">activeDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1cb8e-142">activeDeviceCount</span></span>|<span data-ttu-id="1cb8e-143">Int32</span><span class="sxs-lookup"><span data-stu-id="1cb8e-143">Int32</span></span>|<span data-ttu-id="1cb8e-144">Количество устройств, на которых приложение было активным.</span><span class="sxs-lookup"><span data-stu-id="1cb8e-144">The number of devices where the app has been active.</span></span> <span data-ttu-id="1cb8e-145">Допустимые значения -2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="1cb8e-145">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="1cb8e-146">appName</span><span class="sxs-lookup"><span data-stu-id="1cb8e-146">appName</span></span>|<span data-ttu-id="1cb8e-147">String</span><span class="sxs-lookup"><span data-stu-id="1cb8e-147">String</span></span>|<span data-ttu-id="1cb8e-148">Имя приложения.</span><span class="sxs-lookup"><span data-stu-id="1cb8e-148">The name of the application.</span></span>|
|<span data-ttu-id="1cb8e-149">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="1cb8e-149">appDisplayName</span></span>|<span data-ttu-id="1cb8e-150">String</span><span class="sxs-lookup"><span data-stu-id="1cb8e-150">String</span></span>|<span data-ttu-id="1cb8e-151">Удобное имя приложения.</span><span class="sxs-lookup"><span data-stu-id="1cb8e-151">The friendly name of the application.</span></span>|
|<span data-ttu-id="1cb8e-152">appPublisher</span><span class="sxs-lookup"><span data-stu-id="1cb8e-152">appPublisher</span></span>|<span data-ttu-id="1cb8e-153">Строка</span><span class="sxs-lookup"><span data-stu-id="1cb8e-153">String</span></span>|<span data-ttu-id="1cb8e-154">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="1cb8e-154">The publisher of the application.</span></span>|
|<span data-ttu-id="1cb8e-155">appUsageDuration</span><span class="sxs-lookup"><span data-stu-id="1cb8e-155">appUsageDuration</span></span>|<span data-ttu-id="1cb8e-156">Int32</span><span class="sxs-lookup"><span data-stu-id="1cb8e-156">Int32</span></span>|<span data-ttu-id="1cb8e-157">Общее время использования приложения в минутах.</span><span class="sxs-lookup"><span data-stu-id="1cb8e-157">The total usage time of the application in minutes.</span></span> <span data-ttu-id="1cb8e-158">Допустимые значения -2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="1cb8e-158">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="1cb8e-159">appCrashCount</span><span class="sxs-lookup"><span data-stu-id="1cb8e-159">appCrashCount</span></span>|<span data-ttu-id="1cb8e-160">Int32</span><span class="sxs-lookup"><span data-stu-id="1cb8e-160">Int32</span></span>|<span data-ttu-id="1cb8e-161">Количество сбоей для приложения.</span><span class="sxs-lookup"><span data-stu-id="1cb8e-161">The number of crashes for the app.</span></span> <span data-ttu-id="1cb8e-162">Допустимые значения -2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="1cb8e-162">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="1cb8e-163">meanTimeToFailureInMinutes</span><span class="sxs-lookup"><span data-stu-id="1cb8e-163">meanTimeToFailureInMinutes</span></span>|<span data-ttu-id="1cb8e-164">Int32</span><span class="sxs-lookup"><span data-stu-id="1cb8e-164">Int32</span></span>|<span data-ttu-id="1cb8e-165">Время сбоя для приложения в минутах.</span><span class="sxs-lookup"><span data-stu-id="1cb8e-165">The mean time to failure for the app in minutes.</span></span> <span data-ttu-id="1cb8e-166">Допустимые значения -2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="1cb8e-166">Valid values -2147483648 to 2147483647</span></span>|



## <a name="response"></a><span data-ttu-id="1cb8e-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="1cb8e-167">Response</span></span>
<span data-ttu-id="1cb8e-168">В случае успеха этот метод возвращает код отклика и объект `201 Created` [userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="1cb8e-168">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1cb8e-169">Пример</span><span class="sxs-lookup"><span data-stu-id="1cb8e-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="1cb8e-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="1cb8e-170">Request</span></span>
<span data-ttu-id="1cb8e-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1cb8e-171">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformanceByOSVersion
Content-type: application/json
Content-length: 415

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthAppPerformanceByOSVersion",
  "osVersion": "Os Version value",
  "osBuildNumber": "Os Build Number value",
  "activeDeviceCount": 1,
  "appName": "App Name value",
  "appDisplayName": "App Display Name value",
  "appPublisher": "App Publisher value",
  "appUsageDuration": 0,
  "appCrashCount": 13,
  "meanTimeToFailureInMinutes": 10
}
```

### <a name="response"></a><span data-ttu-id="1cb8e-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="1cb8e-172">Response</span></span>
<span data-ttu-id="1cb8e-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1cb8e-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 464

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthAppPerformanceByOSVersion",
  "id": "65f9bde9-bde9-65f9-e9bd-f965e9bdf965",
  "osVersion": "Os Version value",
  "osBuildNumber": "Os Build Number value",
  "activeDeviceCount": 1,
  "appName": "App Name value",
  "appDisplayName": "App Display Name value",
  "appPublisher": "App Publisher value",
  "appUsageDuration": 0,
  "appCrashCount": 13,
  "meanTimeToFailureInMinutes": 10
}
```




