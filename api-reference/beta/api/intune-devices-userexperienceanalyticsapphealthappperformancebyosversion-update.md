---
title: Обновление Усерекспериенцеаналитиксапфеалсаппперформанцебйосверсион
description: Обновление свойств объекта Усерекспериенцеаналитиксапфеалсаппперформанцебйосверсион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f6cb3dd4467dd35be8518aaddf1ff5028d0406d4
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48732249"
---
# <a name="update-userexperienceanalyticsapphealthappperformancebyosversion"></a><span data-ttu-id="c431b-103">Обновление Усерекспериенцеаналитиксапфеалсаппперформанцебйосверсион</span><span class="sxs-lookup"><span data-stu-id="c431b-103">Update userExperienceAnalyticsAppHealthAppPerformanceByOSVersion</span></span>

<span data-ttu-id="c431b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c431b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c431b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c431b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c431b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c431b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c431b-107">Обновление свойств объекта [усерекспериенцеаналитиксапфеалсаппперформанцебйосверсион](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md) .</span><span class="sxs-lookup"><span data-stu-id="c431b-107">Update the properties of a [userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c431b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c431b-108">Prerequisites</span></span>
<span data-ttu-id="c431b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c431b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c431b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c431b-111">Permission type</span></span>|<span data-ttu-id="c431b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c431b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c431b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c431b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c431b-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c431b-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c431b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c431b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c431b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c431b-116">Not supported.</span></span>|
|<span data-ttu-id="c431b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c431b-117">Application</span></span>|<span data-ttu-id="c431b-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c431b-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c431b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c431b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformanceByOSVersion/{userExperienceAnalyticsAppHealthAppPerformanceByOSVersionId}
```

## <a name="request-headers"></a><span data-ttu-id="c431b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c431b-120">Request headers</span></span>
|<span data-ttu-id="c431b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c431b-121">Header</span></span>|<span data-ttu-id="c431b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c431b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c431b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c431b-123">Authorization</span></span>|<span data-ttu-id="c431b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c431b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c431b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c431b-125">Accept</span></span>|<span data-ttu-id="c431b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c431b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c431b-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c431b-127">Request body</span></span>
<span data-ttu-id="c431b-128">В тексте запроса добавьте представление объекта [усерекспериенцеаналитиксапфеалсаппперформанцебйосверсион](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c431b-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md) object.</span></span>

<span data-ttu-id="c431b-129">В следующей таблице приведены свойства, необходимые при создании [усерекспериенцеаналитиксапфеалсаппперформанцебйосверсион](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md).</span><span class="sxs-lookup"><span data-stu-id="c431b-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md).</span></span>

|<span data-ttu-id="c431b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c431b-130">Property</span></span>|<span data-ttu-id="c431b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c431b-131">Type</span></span>|<span data-ttu-id="c431b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c431b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c431b-133">id</span><span class="sxs-lookup"><span data-stu-id="c431b-133">id</span></span>|<span data-ttu-id="c431b-134">Строка</span><span class="sxs-lookup"><span data-stu-id="c431b-134">String</span></span>|<span data-ttu-id="c431b-135">Уникальный идентификатор объекта производительности "версия приложения аналитики взаимодействия с пользователем".</span><span class="sxs-lookup"><span data-stu-id="c431b-135">The unique identifier of the user experience analytics app version performance object.</span></span>|
|<span data-ttu-id="c431b-136">osVersion</span><span class="sxs-lookup"><span data-stu-id="c431b-136">osVersion</span></span>|<span data-ttu-id="c431b-137">String</span><span class="sxs-lookup"><span data-stu-id="c431b-137">String</span></span>|<span data-ttu-id="c431b-138">Версия операционной системы приложения.</span><span class="sxs-lookup"><span data-stu-id="c431b-138">The os version of the application.</span></span>|
|<span data-ttu-id="c431b-139">осбуилднумбер</span><span class="sxs-lookup"><span data-stu-id="c431b-139">osBuildNumber</span></span>|<span data-ttu-id="c431b-140">Строка</span><span class="sxs-lookup"><span data-stu-id="c431b-140">String</span></span>|<span data-ttu-id="c431b-141">Номер сборки ОС приложения.</span><span class="sxs-lookup"><span data-stu-id="c431b-141">The os build number of the application.</span></span>|
|<span data-ttu-id="c431b-142">активедевицекаунт</span><span class="sxs-lookup"><span data-stu-id="c431b-142">activeDeviceCount</span></span>|<span data-ttu-id="c431b-143">Int32</span><span class="sxs-lookup"><span data-stu-id="c431b-143">Int32</span></span>|<span data-ttu-id="c431b-144">Количество устройств, в которых приложение было активно.</span><span class="sxs-lookup"><span data-stu-id="c431b-144">The number of devices where the app has been active.</span></span> <span data-ttu-id="c431b-145">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="c431b-145">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="c431b-146">appName</span><span class="sxs-lookup"><span data-stu-id="c431b-146">appName</span></span>|<span data-ttu-id="c431b-147">String</span><span class="sxs-lookup"><span data-stu-id="c431b-147">String</span></span>|<span data-ttu-id="c431b-148">Имя приложения.</span><span class="sxs-lookup"><span data-stu-id="c431b-148">The name of the application.</span></span>|
|<span data-ttu-id="c431b-149">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="c431b-149">appDisplayName</span></span>|<span data-ttu-id="c431b-150">String</span><span class="sxs-lookup"><span data-stu-id="c431b-150">String</span></span>|<span data-ttu-id="c431b-151">Понятное имя приложения.</span><span class="sxs-lookup"><span data-stu-id="c431b-151">The friendly name of the application.</span></span>|
|<span data-ttu-id="c431b-152">апппублишер</span><span class="sxs-lookup"><span data-stu-id="c431b-152">appPublisher</span></span>|<span data-ttu-id="c431b-153">Строка</span><span class="sxs-lookup"><span data-stu-id="c431b-153">String</span></span>|<span data-ttu-id="c431b-154">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="c431b-154">The publisher of the application.</span></span>|
|<span data-ttu-id="c431b-155">аппусажедуратион</span><span class="sxs-lookup"><span data-stu-id="c431b-155">appUsageDuration</span></span>|<span data-ttu-id="c431b-156">Int32</span><span class="sxs-lookup"><span data-stu-id="c431b-156">Int32</span></span>|<span data-ttu-id="c431b-157">Общее время использования приложения в минутах.</span><span class="sxs-lookup"><span data-stu-id="c431b-157">The total usage time of the application in minutes.</span></span> <span data-ttu-id="c431b-158">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="c431b-158">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="c431b-159">аппкрашкаунт</span><span class="sxs-lookup"><span data-stu-id="c431b-159">appCrashCount</span></span>|<span data-ttu-id="c431b-160">Int32</span><span class="sxs-lookup"><span data-stu-id="c431b-160">Int32</span></span>|<span data-ttu-id="c431b-161">Число сбоев для приложения.</span><span class="sxs-lookup"><span data-stu-id="c431b-161">The number of crashes for the app.</span></span> <span data-ttu-id="c431b-162">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="c431b-162">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="c431b-163">меантиметофаилуреинминутес</span><span class="sxs-lookup"><span data-stu-id="c431b-163">meanTimeToFailureInMinutes</span></span>|<span data-ttu-id="c431b-164">Int32</span><span class="sxs-lookup"><span data-stu-id="c431b-164">Int32</span></span>|<span data-ttu-id="c431b-165">Среднее время до сбоя приложения в минутах.</span><span class="sxs-lookup"><span data-stu-id="c431b-165">The mean time to failure for the app in minutes.</span></span> <span data-ttu-id="c431b-166">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="c431b-166">Valid values -2147483648 to 2147483647</span></span>|



## <a name="response"></a><span data-ttu-id="c431b-167">Ответ</span><span class="sxs-lookup"><span data-stu-id="c431b-167">Response</span></span>
<span data-ttu-id="c431b-168">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [усерекспериенцеаналитиксапфеалсаппперформанцебйосверсион](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c431b-168">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c431b-169">Пример</span><span class="sxs-lookup"><span data-stu-id="c431b-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="c431b-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="c431b-170">Request</span></span>
<span data-ttu-id="c431b-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c431b-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c431b-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="c431b-172">Response</span></span>
<span data-ttu-id="c431b-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c431b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





