---
title: Обновление userExperienceAnalyticsAppHealthAppPerformanceByOSVersion
description: Обновление свойств объекта userExperienceAnalyticsAppHealthAppPerformanceByOSVersion.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 938626293f576da2ae505b8347cded9785da6c97
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51136218"
---
# <a name="update-userexperienceanalyticsapphealthappperformancebyosversion"></a><span data-ttu-id="d7c27-103">Обновление userExperienceAnalyticsAppHealthAppPerformanceByOSVersion</span><span class="sxs-lookup"><span data-stu-id="d7c27-103">Update userExperienceAnalyticsAppHealthAppPerformanceByOSVersion</span></span>

<span data-ttu-id="d7c27-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7c27-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d7c27-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7c27-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d7c27-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d7c27-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7c27-107">Обновление свойств объекта [userExperienceAnalyticsAppHealthAppPerformanceByOSVersion.](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md)</span><span class="sxs-lookup"><span data-stu-id="d7c27-107">Update the properties of a [userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d7c27-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d7c27-108">Prerequisites</span></span>
<span data-ttu-id="d7c27-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7c27-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7c27-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d7c27-111">Permission type</span></span>|<span data-ttu-id="d7c27-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d7c27-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d7c27-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d7c27-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d7c27-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7c27-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d7c27-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d7c27-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d7c27-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7c27-116">Not supported.</span></span>|
|<span data-ttu-id="d7c27-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="d7c27-117">Application</span></span>|<span data-ttu-id="d7c27-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7c27-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d7c27-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d7c27-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformanceByOSVersion/{userExperienceAnalyticsAppHealthAppPerformanceByOSVersionId}
```

## <a name="request-headers"></a><span data-ttu-id="d7c27-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d7c27-120">Request headers</span></span>
|<span data-ttu-id="d7c27-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d7c27-121">Header</span></span>|<span data-ttu-id="d7c27-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d7c27-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d7c27-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7c27-123">Authorization</span></span>|<span data-ttu-id="d7c27-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d7c27-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d7c27-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d7c27-125">Accept</span></span>|<span data-ttu-id="d7c27-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d7c27-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7c27-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d7c27-127">Request body</span></span>
<span data-ttu-id="d7c27-128">В теле запроса поставляем представление JSON для [объекта userExperienceAnalyticsAppHealthAppPerformanceByOSVersion.](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md)</span><span class="sxs-lookup"><span data-stu-id="d7c27-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md) object.</span></span>

<span data-ttu-id="d7c27-129">В следующей таблице показаны свойства, необходимые при создании [userExperienceAnalyticsAppHealthAppPerformanceByOSVersion.](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md)</span><span class="sxs-lookup"><span data-stu-id="d7c27-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md).</span></span>

|<span data-ttu-id="d7c27-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d7c27-130">Property</span></span>|<span data-ttu-id="d7c27-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d7c27-131">Type</span></span>|<span data-ttu-id="d7c27-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d7c27-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7c27-133">id</span><span class="sxs-lookup"><span data-stu-id="d7c27-133">id</span></span>|<span data-ttu-id="d7c27-134">Строка</span><span class="sxs-lookup"><span data-stu-id="d7c27-134">String</span></span>|<span data-ttu-id="d7c27-135">Уникальный идентификатор объекта производительности версии версии пользовательского интерфейса для аналитики приложений.</span><span class="sxs-lookup"><span data-stu-id="d7c27-135">The unique identifier of the user experience analytics app version performance object.</span></span>|
|<span data-ttu-id="d7c27-136">osVersion</span><span class="sxs-lookup"><span data-stu-id="d7c27-136">osVersion</span></span>|<span data-ttu-id="d7c27-137">String</span><span class="sxs-lookup"><span data-stu-id="d7c27-137">String</span></span>|<span data-ttu-id="d7c27-138">Версия ос приложения.</span><span class="sxs-lookup"><span data-stu-id="d7c27-138">The os version of the application.</span></span>|
|<span data-ttu-id="d7c27-139">osBuildNumber</span><span class="sxs-lookup"><span data-stu-id="d7c27-139">osBuildNumber</span></span>|<span data-ttu-id="d7c27-140">Строка</span><span class="sxs-lookup"><span data-stu-id="d7c27-140">String</span></span>|<span data-ttu-id="d7c27-141">Число сборки ос приложения.</span><span class="sxs-lookup"><span data-stu-id="d7c27-141">The os build number of the application.</span></span>|
|<span data-ttu-id="d7c27-142">activeDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d7c27-142">activeDeviceCount</span></span>|<span data-ttu-id="d7c27-143">Int32</span><span class="sxs-lookup"><span data-stu-id="d7c27-143">Int32</span></span>|<span data-ttu-id="d7c27-144">Количество устройств, на которых приложение было активным.</span><span class="sxs-lookup"><span data-stu-id="d7c27-144">The number of devices where the app has been active.</span></span> <span data-ttu-id="d7c27-145">Допустимые значения -2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="d7c27-145">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="d7c27-146">appName</span><span class="sxs-lookup"><span data-stu-id="d7c27-146">appName</span></span>|<span data-ttu-id="d7c27-147">String</span><span class="sxs-lookup"><span data-stu-id="d7c27-147">String</span></span>|<span data-ttu-id="d7c27-148">Имя приложения.</span><span class="sxs-lookup"><span data-stu-id="d7c27-148">The name of the application.</span></span>|
|<span data-ttu-id="d7c27-149">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="d7c27-149">appDisplayName</span></span>|<span data-ttu-id="d7c27-150">String</span><span class="sxs-lookup"><span data-stu-id="d7c27-150">String</span></span>|<span data-ttu-id="d7c27-151">Удобное имя приложения.</span><span class="sxs-lookup"><span data-stu-id="d7c27-151">The friendly name of the application.</span></span>|
|<span data-ttu-id="d7c27-152">appPublisher</span><span class="sxs-lookup"><span data-stu-id="d7c27-152">appPublisher</span></span>|<span data-ttu-id="d7c27-153">Строка</span><span class="sxs-lookup"><span data-stu-id="d7c27-153">String</span></span>|<span data-ttu-id="d7c27-154">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="d7c27-154">The publisher of the application.</span></span>|
|<span data-ttu-id="d7c27-155">appUsageDuration</span><span class="sxs-lookup"><span data-stu-id="d7c27-155">appUsageDuration</span></span>|<span data-ttu-id="d7c27-156">Int32</span><span class="sxs-lookup"><span data-stu-id="d7c27-156">Int32</span></span>|<span data-ttu-id="d7c27-157">Общее время использования приложения в минутах.</span><span class="sxs-lookup"><span data-stu-id="d7c27-157">The total usage time of the application in minutes.</span></span> <span data-ttu-id="d7c27-158">Допустимые значения -2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="d7c27-158">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="d7c27-159">appCrashCount</span><span class="sxs-lookup"><span data-stu-id="d7c27-159">appCrashCount</span></span>|<span data-ttu-id="d7c27-160">Int32</span><span class="sxs-lookup"><span data-stu-id="d7c27-160">Int32</span></span>|<span data-ttu-id="d7c27-161">Количество сбоей для приложения.</span><span class="sxs-lookup"><span data-stu-id="d7c27-161">The number of crashes for the app.</span></span> <span data-ttu-id="d7c27-162">Допустимые значения -2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="d7c27-162">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="d7c27-163">meanTimeToFailureInMinutes</span><span class="sxs-lookup"><span data-stu-id="d7c27-163">meanTimeToFailureInMinutes</span></span>|<span data-ttu-id="d7c27-164">Int32</span><span class="sxs-lookup"><span data-stu-id="d7c27-164">Int32</span></span>|<span data-ttu-id="d7c27-165">Время сбоя для приложения в минутах.</span><span class="sxs-lookup"><span data-stu-id="d7c27-165">The mean time to failure for the app in minutes.</span></span> <span data-ttu-id="d7c27-166">Допустимые значения -2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="d7c27-166">Valid values -2147483648 to 2147483647</span></span>|



## <a name="response"></a><span data-ttu-id="d7c27-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7c27-167">Response</span></span>
<span data-ttu-id="d7c27-168">В случае успеха этот метод возвращает код отклика и обновленный `200 OK` [объект userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d7c27-168">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7c27-169">Пример</span><span class="sxs-lookup"><span data-stu-id="d7c27-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="d7c27-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="d7c27-170">Request</span></span>
<span data-ttu-id="d7c27-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d7c27-171">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformanceByOSVersion/{userExperienceAnalyticsAppHealthAppPerformanceByOSVersionId}
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

### <a name="response"></a><span data-ttu-id="d7c27-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7c27-172">Response</span></span>
<span data-ttu-id="d7c27-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d7c27-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




