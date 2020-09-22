---
title: Создание Усерекспериенцеаналитиксапфеалсаппперформанцебяппверсион
description: Создание нового объекта Усерекспериенцеаналитиксапфеалсаппперформанцебяппверсион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f02aaede3a622fa8cd715e37eaa200e5befadaa6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48023636"
---
# <a name="create-userexperienceanalyticsapphealthappperformancebyappversion"></a><span data-ttu-id="9f287-103">Создание Усерекспериенцеаналитиксапфеалсаппперформанцебяппверсион</span><span class="sxs-lookup"><span data-stu-id="9f287-103">Create userExperienceAnalyticsAppHealthAppPerformanceByAppVersion</span></span>

<span data-ttu-id="9f287-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f287-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9f287-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f287-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9f287-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9f287-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f287-107">Создание нового объекта [усерекспериенцеаналитиксапфеалсаппперформанцебяппверсион](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) .</span><span class="sxs-lookup"><span data-stu-id="9f287-107">Create a new [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9f287-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9f287-108">Prerequisites</span></span>
<span data-ttu-id="9f287-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f287-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f287-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9f287-111">Permission type</span></span>|<span data-ttu-id="9f287-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9f287-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f287-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9f287-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9f287-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f287-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="9f287-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f287-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f287-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f287-116">Not supported.</span></span>|
|<span data-ttu-id="9f287-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9f287-117">Application</span></span>|<span data-ttu-id="9f287-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f287-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f287-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9f287-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformanceByAppVersion
```

## <a name="request-headers"></a><span data-ttu-id="9f287-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9f287-120">Request headers</span></span>
|<span data-ttu-id="9f287-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9f287-121">Header</span></span>|<span data-ttu-id="9f287-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9f287-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f287-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f287-123">Authorization</span></span>|<span data-ttu-id="9f287-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9f287-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f287-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9f287-125">Accept</span></span>|<span data-ttu-id="9f287-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9f287-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f287-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9f287-127">Request body</span></span>
<span data-ttu-id="9f287-128">В тексте запроса добавьте представление объекта Усерекспериенцеаналитиксапфеалсаппперформанцебяппверсион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9f287-128">In the request body, supply a JSON representation for the userExperienceAnalyticsAppHealthAppPerformanceByAppVersion object.</span></span>

<span data-ttu-id="9f287-129">В следующей таблице приведены свойства, необходимые при создании Усерекспериенцеаналитиксапфеалсаппперформанцебяппверсион.</span><span class="sxs-lookup"><span data-stu-id="9f287-129">The following table shows the properties that are required when you create the userExperienceAnalyticsAppHealthAppPerformanceByAppVersion.</span></span>

|<span data-ttu-id="9f287-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9f287-130">Property</span></span>|<span data-ttu-id="9f287-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9f287-131">Type</span></span>|<span data-ttu-id="9f287-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9f287-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f287-133">id</span><span class="sxs-lookup"><span data-stu-id="9f287-133">id</span></span>|<span data-ttu-id="9f287-134">String</span><span class="sxs-lookup"><span data-stu-id="9f287-134">String</span></span>|<span data-ttu-id="9f287-135">Уникальный идентификатор объекта производительности приложения аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="9f287-135">The unique identifier of the user experience analytics app performance object.</span></span>|
|<span data-ttu-id="9f287-136">аппверсион</span><span class="sxs-lookup"><span data-stu-id="9f287-136">appVersion</span></span>|<span data-ttu-id="9f287-137">String</span><span class="sxs-lookup"><span data-stu-id="9f287-137">String</span></span>|<span data-ttu-id="9f287-138">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="9f287-138">The version of the application.</span></span>|
|<span data-ttu-id="9f287-139">appName</span><span class="sxs-lookup"><span data-stu-id="9f287-139">appName</span></span>|<span data-ttu-id="9f287-140">String</span><span class="sxs-lookup"><span data-stu-id="9f287-140">String</span></span>|<span data-ttu-id="9f287-141">Имя приложения.</span><span class="sxs-lookup"><span data-stu-id="9f287-141">The name of the application.</span></span>|
|<span data-ttu-id="9f287-142">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="9f287-142">appDisplayName</span></span>|<span data-ttu-id="9f287-143">String</span><span class="sxs-lookup"><span data-stu-id="9f287-143">String</span></span>|<span data-ttu-id="9f287-144">Понятное имя приложения.</span><span class="sxs-lookup"><span data-stu-id="9f287-144">The friendly name of the application.</span></span>|
|<span data-ttu-id="9f287-145">апппублишер</span><span class="sxs-lookup"><span data-stu-id="9f287-145">appPublisher</span></span>|<span data-ttu-id="9f287-146">String</span><span class="sxs-lookup"><span data-stu-id="9f287-146">String</span></span>|<span data-ttu-id="9f287-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="9f287-147">The publisher of the application.</span></span>|
|<span data-ttu-id="9f287-148">аппусажедуратион</span><span class="sxs-lookup"><span data-stu-id="9f287-148">appUsageDuration</span></span>|<span data-ttu-id="9f287-149">Int32</span><span class="sxs-lookup"><span data-stu-id="9f287-149">Int32</span></span>|<span data-ttu-id="9f287-150">Общее время использования приложения в минутах.</span><span class="sxs-lookup"><span data-stu-id="9f287-150">The total usage time of the application in minutes.</span></span> <span data-ttu-id="9f287-151">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="9f287-151">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="9f287-152">аппкрашкаунт</span><span class="sxs-lookup"><span data-stu-id="9f287-152">appCrashCount</span></span>|<span data-ttu-id="9f287-153">Int32</span><span class="sxs-lookup"><span data-stu-id="9f287-153">Int32</span></span>|<span data-ttu-id="9f287-154">Число сбоев для приложения.</span><span class="sxs-lookup"><span data-stu-id="9f287-154">The number of crashes for the app.</span></span> <span data-ttu-id="9f287-155">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="9f287-155">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="9f287-156">меантиметофаилуреинминутес</span><span class="sxs-lookup"><span data-stu-id="9f287-156">meanTimeToFailureInMinutes</span></span>|<span data-ttu-id="9f287-157">Int32</span><span class="sxs-lookup"><span data-stu-id="9f287-157">Int32</span></span>|<span data-ttu-id="9f287-158">Среднее время до сбоя приложения в минутах.</span><span class="sxs-lookup"><span data-stu-id="9f287-158">The mean time to failure for the app in minutes.</span></span> <span data-ttu-id="9f287-159">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="9f287-159">Valid values -2147483648 to 2147483647</span></span>|



## <a name="response"></a><span data-ttu-id="9f287-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f287-160">Response</span></span>
<span data-ttu-id="9f287-161">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [усерекспериенцеаналитиксапфеалсаппперформанцебяппверсион](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9f287-161">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f287-162">Пример</span><span class="sxs-lookup"><span data-stu-id="9f287-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="9f287-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="9f287-163">Request</span></span>
<span data-ttu-id="9f287-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9f287-164">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformanceByAppVersion
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

### <a name="response"></a><span data-ttu-id="9f287-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f287-165">Response</span></span>
<span data-ttu-id="9f287-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9f287-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






