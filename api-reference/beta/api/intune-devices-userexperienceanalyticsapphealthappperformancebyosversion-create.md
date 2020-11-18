---
title: Создание Усерекспериенцеаналитиксапфеалсаппперформанцебйосверсион
description: Создание нового объекта Усерекспериенцеаналитиксапфеалсаппперформанцебйосверсион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b1c3ac5f96c506e01492c11aaf6c0fef2ea75686
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49203147"
---
# <a name="create-userexperienceanalyticsapphealthappperformancebyosversion"></a><span data-ttu-id="96338-103">Создание Усерекспериенцеаналитиксапфеалсаппперформанцебйосверсион</span><span class="sxs-lookup"><span data-stu-id="96338-103">Create userExperienceAnalyticsAppHealthAppPerformanceByOSVersion</span></span>

<span data-ttu-id="96338-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96338-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="96338-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96338-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="96338-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="96338-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96338-107">Создание нового объекта [усерекспериенцеаналитиксапфеалсаппперформанцебйосверсион](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md) .</span><span class="sxs-lookup"><span data-stu-id="96338-107">Create a new [userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="96338-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="96338-108">Prerequisites</span></span>
<span data-ttu-id="96338-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96338-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96338-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="96338-111">Permission type</span></span>|<span data-ttu-id="96338-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="96338-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="96338-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="96338-113">Delegated (work or school account)</span></span>|<span data-ttu-id="96338-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96338-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="96338-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="96338-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96338-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96338-116">Not supported.</span></span>|
|<span data-ttu-id="96338-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="96338-117">Application</span></span>|<span data-ttu-id="96338-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96338-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="96338-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="96338-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformanceByOSVersion
```

## <a name="request-headers"></a><span data-ttu-id="96338-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="96338-120">Request headers</span></span>
|<span data-ttu-id="96338-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="96338-121">Header</span></span>|<span data-ttu-id="96338-122">Значение</span><span class="sxs-lookup"><span data-stu-id="96338-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="96338-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="96338-123">Authorization</span></span>|<span data-ttu-id="96338-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="96338-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="96338-125">Accept</span><span class="sxs-lookup"><span data-stu-id="96338-125">Accept</span></span>|<span data-ttu-id="96338-126">application/json</span><span class="sxs-lookup"><span data-stu-id="96338-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="96338-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="96338-127">Request body</span></span>
<span data-ttu-id="96338-128">В тексте запроса добавьте представление объекта Усерекспериенцеаналитиксапфеалсаппперформанцебйосверсион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="96338-128">In the request body, supply a JSON representation for the userExperienceAnalyticsAppHealthAppPerformanceByOSVersion object.</span></span>

<span data-ttu-id="96338-129">В следующей таблице приведены свойства, необходимые при создании Усерекспериенцеаналитиксапфеалсаппперформанцебйосверсион.</span><span class="sxs-lookup"><span data-stu-id="96338-129">The following table shows the properties that are required when you create the userExperienceAnalyticsAppHealthAppPerformanceByOSVersion.</span></span>

|<span data-ttu-id="96338-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="96338-130">Property</span></span>|<span data-ttu-id="96338-131">Тип</span><span class="sxs-lookup"><span data-stu-id="96338-131">Type</span></span>|<span data-ttu-id="96338-132">Описание</span><span class="sxs-lookup"><span data-stu-id="96338-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96338-133">id</span><span class="sxs-lookup"><span data-stu-id="96338-133">id</span></span>|<span data-ttu-id="96338-134">String</span><span class="sxs-lookup"><span data-stu-id="96338-134">String</span></span>|<span data-ttu-id="96338-135">Уникальный идентификатор объекта производительности "версия приложения аналитики взаимодействия с пользователем".</span><span class="sxs-lookup"><span data-stu-id="96338-135">The unique identifier of the user experience analytics app version performance object.</span></span>|
|<span data-ttu-id="96338-136">osVersion</span><span class="sxs-lookup"><span data-stu-id="96338-136">osVersion</span></span>|<span data-ttu-id="96338-137">String</span><span class="sxs-lookup"><span data-stu-id="96338-137">String</span></span>|<span data-ttu-id="96338-138">Версия операционной системы приложения.</span><span class="sxs-lookup"><span data-stu-id="96338-138">The os version of the application.</span></span>|
|<span data-ttu-id="96338-139">осбуилднумбер</span><span class="sxs-lookup"><span data-stu-id="96338-139">osBuildNumber</span></span>|<span data-ttu-id="96338-140">String</span><span class="sxs-lookup"><span data-stu-id="96338-140">String</span></span>|<span data-ttu-id="96338-141">Номер сборки ОС приложения.</span><span class="sxs-lookup"><span data-stu-id="96338-141">The os build number of the application.</span></span>|
|<span data-ttu-id="96338-142">активедевицекаунт</span><span class="sxs-lookup"><span data-stu-id="96338-142">activeDeviceCount</span></span>|<span data-ttu-id="96338-143">Int32</span><span class="sxs-lookup"><span data-stu-id="96338-143">Int32</span></span>|<span data-ttu-id="96338-144">Количество устройств, в которых приложение было активно.</span><span class="sxs-lookup"><span data-stu-id="96338-144">The number of devices where the app has been active.</span></span> <span data-ttu-id="96338-145">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="96338-145">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="96338-146">appName</span><span class="sxs-lookup"><span data-stu-id="96338-146">appName</span></span>|<span data-ttu-id="96338-147">String</span><span class="sxs-lookup"><span data-stu-id="96338-147">String</span></span>|<span data-ttu-id="96338-148">Имя приложения.</span><span class="sxs-lookup"><span data-stu-id="96338-148">The name of the application.</span></span>|
|<span data-ttu-id="96338-149">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="96338-149">appDisplayName</span></span>|<span data-ttu-id="96338-150">String</span><span class="sxs-lookup"><span data-stu-id="96338-150">String</span></span>|<span data-ttu-id="96338-151">Понятное имя приложения.</span><span class="sxs-lookup"><span data-stu-id="96338-151">The friendly name of the application.</span></span>|
|<span data-ttu-id="96338-152">апппублишер</span><span class="sxs-lookup"><span data-stu-id="96338-152">appPublisher</span></span>|<span data-ttu-id="96338-153">String</span><span class="sxs-lookup"><span data-stu-id="96338-153">String</span></span>|<span data-ttu-id="96338-154">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="96338-154">The publisher of the application.</span></span>|
|<span data-ttu-id="96338-155">аппусажедуратион</span><span class="sxs-lookup"><span data-stu-id="96338-155">appUsageDuration</span></span>|<span data-ttu-id="96338-156">Int32</span><span class="sxs-lookup"><span data-stu-id="96338-156">Int32</span></span>|<span data-ttu-id="96338-157">Общее время использования приложения в минутах.</span><span class="sxs-lookup"><span data-stu-id="96338-157">The total usage time of the application in minutes.</span></span> <span data-ttu-id="96338-158">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="96338-158">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="96338-159">аппкрашкаунт</span><span class="sxs-lookup"><span data-stu-id="96338-159">appCrashCount</span></span>|<span data-ttu-id="96338-160">Int32</span><span class="sxs-lookup"><span data-stu-id="96338-160">Int32</span></span>|<span data-ttu-id="96338-161">Число сбоев для приложения.</span><span class="sxs-lookup"><span data-stu-id="96338-161">The number of crashes for the app.</span></span> <span data-ttu-id="96338-162">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="96338-162">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="96338-163">меантиметофаилуреинминутес</span><span class="sxs-lookup"><span data-stu-id="96338-163">meanTimeToFailureInMinutes</span></span>|<span data-ttu-id="96338-164">Int32</span><span class="sxs-lookup"><span data-stu-id="96338-164">Int32</span></span>|<span data-ttu-id="96338-165">Среднее время до сбоя приложения в минутах.</span><span class="sxs-lookup"><span data-stu-id="96338-165">The mean time to failure for the app in minutes.</span></span> <span data-ttu-id="96338-166">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="96338-166">Valid values -2147483648 to 2147483647</span></span>|



## <a name="response"></a><span data-ttu-id="96338-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="96338-167">Response</span></span>
<span data-ttu-id="96338-168">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [усерекспериенцеаналитиксапфеалсаппперформанцебйосверсион](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="96338-168">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96338-169">Пример</span><span class="sxs-lookup"><span data-stu-id="96338-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="96338-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="96338-170">Request</span></span>
<span data-ttu-id="96338-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="96338-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="96338-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="96338-172">Response</span></span>
<span data-ttu-id="96338-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="96338-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




