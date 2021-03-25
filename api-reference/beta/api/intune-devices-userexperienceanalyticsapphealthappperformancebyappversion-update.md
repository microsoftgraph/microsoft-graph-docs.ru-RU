---
title: Обновление userExperienceAnalyticsAppHealthAppPerformanceByAppVersion
description: Обновление свойств объекта userExperienceAnalyticsAppHealthAppPerformanceByAppVersion.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 41649f902158b198d7edcd0687e49d9c6d65dacb
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51158040"
---
# <a name="update-userexperienceanalyticsapphealthappperformancebyappversion"></a><span data-ttu-id="ab654-103">Обновление userExperienceAnalyticsAppHealthAppPerformanceByAppVersion</span><span class="sxs-lookup"><span data-stu-id="ab654-103">Update userExperienceAnalyticsAppHealthAppPerformanceByAppVersion</span></span>

<span data-ttu-id="ab654-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ab654-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ab654-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab654-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ab654-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ab654-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab654-107">Обновление свойств объекта [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion.](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md)</span><span class="sxs-lookup"><span data-stu-id="ab654-107">Update the properties of a [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ab654-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ab654-108">Prerequisites</span></span>
<span data-ttu-id="ab654-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab654-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab654-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ab654-111">Permission type</span></span>|<span data-ttu-id="ab654-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ab654-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ab654-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ab654-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ab654-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab654-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ab654-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ab654-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ab654-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab654-116">Not supported.</span></span>|
|<span data-ttu-id="ab654-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="ab654-117">Application</span></span>|<span data-ttu-id="ab654-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab654-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ab654-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ab654-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformanceByAppVersion/{userExperienceAnalyticsAppHealthAppPerformanceByAppVersionId}
```

## <a name="request-headers"></a><span data-ttu-id="ab654-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ab654-120">Request headers</span></span>
|<span data-ttu-id="ab654-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ab654-121">Header</span></span>|<span data-ttu-id="ab654-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ab654-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ab654-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab654-123">Authorization</span></span>|<span data-ttu-id="ab654-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ab654-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ab654-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ab654-125">Accept</span></span>|<span data-ttu-id="ab654-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ab654-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab654-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ab654-127">Request body</span></span>
<span data-ttu-id="ab654-128">В теле запроса поставляем представление JSON для [объекта userExperienceAnalyticsAppHealthAppPerformanceByAppVersion.](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md)</span><span class="sxs-lookup"><span data-stu-id="ab654-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) object.</span></span>

<span data-ttu-id="ab654-129">В следующей таблице показаны свойства, необходимые при создании [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion.](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md)</span><span class="sxs-lookup"><span data-stu-id="ab654-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md).</span></span>

|<span data-ttu-id="ab654-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ab654-130">Property</span></span>|<span data-ttu-id="ab654-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ab654-131">Type</span></span>|<span data-ttu-id="ab654-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ab654-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab654-133">id</span><span class="sxs-lookup"><span data-stu-id="ab654-133">id</span></span>|<span data-ttu-id="ab654-134">Строка</span><span class="sxs-lookup"><span data-stu-id="ab654-134">String</span></span>|<span data-ttu-id="ab654-135">Уникальный идентификатор объекта производительности приложения для аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="ab654-135">The unique identifier of the user experience analytics app performance object.</span></span>|
|<span data-ttu-id="ab654-136">appVersion</span><span class="sxs-lookup"><span data-stu-id="ab654-136">appVersion</span></span>|<span data-ttu-id="ab654-137">Строка</span><span class="sxs-lookup"><span data-stu-id="ab654-137">String</span></span>|<span data-ttu-id="ab654-138">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="ab654-138">The version of the application.</span></span>|
|<span data-ttu-id="ab654-139">appName</span><span class="sxs-lookup"><span data-stu-id="ab654-139">appName</span></span>|<span data-ttu-id="ab654-140">String</span><span class="sxs-lookup"><span data-stu-id="ab654-140">String</span></span>|<span data-ttu-id="ab654-141">Имя приложения.</span><span class="sxs-lookup"><span data-stu-id="ab654-141">The name of the application.</span></span>|
|<span data-ttu-id="ab654-142">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="ab654-142">appDisplayName</span></span>|<span data-ttu-id="ab654-143">String</span><span class="sxs-lookup"><span data-stu-id="ab654-143">String</span></span>|<span data-ttu-id="ab654-144">Удобное имя приложения.</span><span class="sxs-lookup"><span data-stu-id="ab654-144">The friendly name of the application.</span></span>|
|<span data-ttu-id="ab654-145">appPublisher</span><span class="sxs-lookup"><span data-stu-id="ab654-145">appPublisher</span></span>|<span data-ttu-id="ab654-146">Строка</span><span class="sxs-lookup"><span data-stu-id="ab654-146">String</span></span>|<span data-ttu-id="ab654-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="ab654-147">The publisher of the application.</span></span>|
|<span data-ttu-id="ab654-148">appUsageDuration</span><span class="sxs-lookup"><span data-stu-id="ab654-148">appUsageDuration</span></span>|<span data-ttu-id="ab654-149">Int32</span><span class="sxs-lookup"><span data-stu-id="ab654-149">Int32</span></span>|<span data-ttu-id="ab654-150">Общее время использования приложения в минутах.</span><span class="sxs-lookup"><span data-stu-id="ab654-150">The total usage time of the application in minutes.</span></span> <span data-ttu-id="ab654-151">Допустимые значения -2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="ab654-151">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="ab654-152">appCrashCount</span><span class="sxs-lookup"><span data-stu-id="ab654-152">appCrashCount</span></span>|<span data-ttu-id="ab654-153">Int32</span><span class="sxs-lookup"><span data-stu-id="ab654-153">Int32</span></span>|<span data-ttu-id="ab654-154">Количество сбоей для приложения.</span><span class="sxs-lookup"><span data-stu-id="ab654-154">The number of crashes for the app.</span></span> <span data-ttu-id="ab654-155">Допустимые значения -2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="ab654-155">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="ab654-156">meanTimeToFailureInMinutes</span><span class="sxs-lookup"><span data-stu-id="ab654-156">meanTimeToFailureInMinutes</span></span>|<span data-ttu-id="ab654-157">Int32</span><span class="sxs-lookup"><span data-stu-id="ab654-157">Int32</span></span>|<span data-ttu-id="ab654-158">Время сбоя для приложения в минутах.</span><span class="sxs-lookup"><span data-stu-id="ab654-158">The mean time to failure for the app in minutes.</span></span> <span data-ttu-id="ab654-159">Допустимые значения -2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="ab654-159">Valid values -2147483648 to 2147483647</span></span>|



## <a name="response"></a><span data-ttu-id="ab654-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="ab654-160">Response</span></span>
<span data-ttu-id="ab654-161">В случае успеха этот метод возвращает код ответа и обновленный объект `200 OK` [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ab654-161">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab654-162">Пример</span><span class="sxs-lookup"><span data-stu-id="ab654-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="ab654-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="ab654-163">Request</span></span>
<span data-ttu-id="ab654-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ab654-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformanceByAppVersion/{userExperienceAnalyticsAppHealthAppPerformanceByAppVersionId}
Content-type: application/json
Content-length: 346

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthAppPerformanceByAppVersion",
  "appVersion": "App Version value",
  "appName": "App Name value",
  "appDisplayName": "App Display Name value",
  "appPublisher": "App Publisher value",
  "appUsageDuration": 0,
  "appCrashCount": 13,
  "meanTimeToFailureInMinutes": 10
}
```

### <a name="response"></a><span data-ttu-id="ab654-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="ab654-165">Response</span></span>
<span data-ttu-id="ab654-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ab654-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 395

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthAppPerformanceByAppVersion",
  "id": "257804c8-04c8-2578-c804-7825c8047825",
  "appVersion": "App Version value",
  "appName": "App Name value",
  "appDisplayName": "App Display Name value",
  "appPublisher": "App Publisher value",
  "appUsageDuration": 0,
  "appCrashCount": 13,
  "meanTimeToFailureInMinutes": 10
}
```




