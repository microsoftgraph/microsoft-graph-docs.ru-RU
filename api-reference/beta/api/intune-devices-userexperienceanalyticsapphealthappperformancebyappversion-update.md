---
title: Обновление Усерекспериенцеаналитиксапфеалсаппперформанцебяппверсион
description: Обновление свойств объекта Усерекспериенцеаналитиксапфеалсаппперформанцебяппверсион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c0c3540478a8fb49413189a13a2bf3021ff6e078
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48735507"
---
# <a name="update-userexperienceanalyticsapphealthappperformancebyappversion"></a><span data-ttu-id="8337f-103">Обновление Усерекспериенцеаналитиксапфеалсаппперформанцебяппверсион</span><span class="sxs-lookup"><span data-stu-id="8337f-103">Update userExperienceAnalyticsAppHealthAppPerformanceByAppVersion</span></span>

<span data-ttu-id="8337f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8337f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8337f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8337f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8337f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8337f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8337f-107">Обновление свойств объекта [усерекспериенцеаналитиксапфеалсаппперформанцебяппверсион](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) .</span><span class="sxs-lookup"><span data-stu-id="8337f-107">Update the properties of a [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8337f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8337f-108">Prerequisites</span></span>
<span data-ttu-id="8337f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8337f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8337f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8337f-111">Permission type</span></span>|<span data-ttu-id="8337f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8337f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8337f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8337f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8337f-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8337f-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8337f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8337f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8337f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8337f-116">Not supported.</span></span>|
|<span data-ttu-id="8337f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8337f-117">Application</span></span>|<span data-ttu-id="8337f-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8337f-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8337f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8337f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformanceByAppVersion/{userExperienceAnalyticsAppHealthAppPerformanceByAppVersionId}
```

## <a name="request-headers"></a><span data-ttu-id="8337f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8337f-120">Request headers</span></span>
|<span data-ttu-id="8337f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8337f-121">Header</span></span>|<span data-ttu-id="8337f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8337f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8337f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8337f-123">Authorization</span></span>|<span data-ttu-id="8337f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8337f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8337f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8337f-125">Accept</span></span>|<span data-ttu-id="8337f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8337f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8337f-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8337f-127">Request body</span></span>
<span data-ttu-id="8337f-128">В тексте запроса добавьте представление объекта [усерекспериенцеаналитиксапфеалсаппперформанцебяппверсион](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8337f-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) object.</span></span>

<span data-ttu-id="8337f-129">В следующей таблице приведены свойства, необходимые при создании [усерекспериенцеаналитиксапфеалсаппперформанцебяппверсион](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md).</span><span class="sxs-lookup"><span data-stu-id="8337f-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md).</span></span>

|<span data-ttu-id="8337f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8337f-130">Property</span></span>|<span data-ttu-id="8337f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8337f-131">Type</span></span>|<span data-ttu-id="8337f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8337f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8337f-133">id</span><span class="sxs-lookup"><span data-stu-id="8337f-133">id</span></span>|<span data-ttu-id="8337f-134">Строка</span><span class="sxs-lookup"><span data-stu-id="8337f-134">String</span></span>|<span data-ttu-id="8337f-135">Уникальный идентификатор объекта производительности приложения аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="8337f-135">The unique identifier of the user experience analytics app performance object.</span></span>|
|<span data-ttu-id="8337f-136">аппверсион</span><span class="sxs-lookup"><span data-stu-id="8337f-136">appVersion</span></span>|<span data-ttu-id="8337f-137">Строка</span><span class="sxs-lookup"><span data-stu-id="8337f-137">String</span></span>|<span data-ttu-id="8337f-138">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="8337f-138">The version of the application.</span></span>|
|<span data-ttu-id="8337f-139">appName</span><span class="sxs-lookup"><span data-stu-id="8337f-139">appName</span></span>|<span data-ttu-id="8337f-140">String</span><span class="sxs-lookup"><span data-stu-id="8337f-140">String</span></span>|<span data-ttu-id="8337f-141">Имя приложения.</span><span class="sxs-lookup"><span data-stu-id="8337f-141">The name of the application.</span></span>|
|<span data-ttu-id="8337f-142">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="8337f-142">appDisplayName</span></span>|<span data-ttu-id="8337f-143">String</span><span class="sxs-lookup"><span data-stu-id="8337f-143">String</span></span>|<span data-ttu-id="8337f-144">Понятное имя приложения.</span><span class="sxs-lookup"><span data-stu-id="8337f-144">The friendly name of the application.</span></span>|
|<span data-ttu-id="8337f-145">апппублишер</span><span class="sxs-lookup"><span data-stu-id="8337f-145">appPublisher</span></span>|<span data-ttu-id="8337f-146">Строка</span><span class="sxs-lookup"><span data-stu-id="8337f-146">String</span></span>|<span data-ttu-id="8337f-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="8337f-147">The publisher of the application.</span></span>|
|<span data-ttu-id="8337f-148">аппусажедуратион</span><span class="sxs-lookup"><span data-stu-id="8337f-148">appUsageDuration</span></span>|<span data-ttu-id="8337f-149">Int32</span><span class="sxs-lookup"><span data-stu-id="8337f-149">Int32</span></span>|<span data-ttu-id="8337f-150">Общее время использования приложения в минутах.</span><span class="sxs-lookup"><span data-stu-id="8337f-150">The total usage time of the application in minutes.</span></span> <span data-ttu-id="8337f-151">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="8337f-151">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="8337f-152">аппкрашкаунт</span><span class="sxs-lookup"><span data-stu-id="8337f-152">appCrashCount</span></span>|<span data-ttu-id="8337f-153">Int32</span><span class="sxs-lookup"><span data-stu-id="8337f-153">Int32</span></span>|<span data-ttu-id="8337f-154">Число сбоев для приложения.</span><span class="sxs-lookup"><span data-stu-id="8337f-154">The number of crashes for the app.</span></span> <span data-ttu-id="8337f-155">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="8337f-155">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="8337f-156">меантиметофаилуреинминутес</span><span class="sxs-lookup"><span data-stu-id="8337f-156">meanTimeToFailureInMinutes</span></span>|<span data-ttu-id="8337f-157">Int32</span><span class="sxs-lookup"><span data-stu-id="8337f-157">Int32</span></span>|<span data-ttu-id="8337f-158">Среднее время до сбоя приложения в минутах.</span><span class="sxs-lookup"><span data-stu-id="8337f-158">The mean time to failure for the app in minutes.</span></span> <span data-ttu-id="8337f-159">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="8337f-159">Valid values -2147483648 to 2147483647</span></span>|



## <a name="response"></a><span data-ttu-id="8337f-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="8337f-160">Response</span></span>
<span data-ttu-id="8337f-161">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [усерекспериенцеаналитиксапфеалсаппперформанцебяппверсион](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8337f-161">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8337f-162">Пример</span><span class="sxs-lookup"><span data-stu-id="8337f-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="8337f-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="8337f-163">Request</span></span>
<span data-ttu-id="8337f-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8337f-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8337f-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="8337f-165">Response</span></span>
<span data-ttu-id="8337f-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8337f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





