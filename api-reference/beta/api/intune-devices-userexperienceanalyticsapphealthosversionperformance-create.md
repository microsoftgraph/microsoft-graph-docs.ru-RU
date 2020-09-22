---
title: Создание Усерекспериенцеаналитиксапфеалсосверсионперформанце
description: Создание нового объекта Усерекспериенцеаналитиксапфеалсосверсионперформанце.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: efb096e85227b9494bb2fd9dae0d50f3123683c1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48023553"
---
# <a name="create-userexperienceanalyticsapphealthosversionperformance"></a><span data-ttu-id="e19dd-103">Создание Усерекспериенцеаналитиксапфеалсосверсионперформанце</span><span class="sxs-lookup"><span data-stu-id="e19dd-103">Create userExperienceAnalyticsAppHealthOSVersionPerformance</span></span>

<span data-ttu-id="e19dd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e19dd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e19dd-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e19dd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e19dd-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e19dd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e19dd-107">Создание нового объекта [усерекспериенцеаналитиксапфеалсосверсионперформанце](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md) .</span><span class="sxs-lookup"><span data-stu-id="e19dd-107">Create a new [userExperienceAnalyticsAppHealthOSVersionPerformance](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e19dd-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e19dd-108">Prerequisites</span></span>
<span data-ttu-id="e19dd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e19dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e19dd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e19dd-111">Permission type</span></span>|<span data-ttu-id="e19dd-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e19dd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e19dd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e19dd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e19dd-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e19dd-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e19dd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e19dd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e19dd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e19dd-116">Not supported.</span></span>|
|<span data-ttu-id="e19dd-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e19dd-117">Application</span></span>|<span data-ttu-id="e19dd-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e19dd-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e19dd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e19dd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsAppHealthOSVersionPerformance
```

## <a name="request-headers"></a><span data-ttu-id="e19dd-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e19dd-120">Request headers</span></span>
|<span data-ttu-id="e19dd-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e19dd-121">Header</span></span>|<span data-ttu-id="e19dd-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e19dd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e19dd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e19dd-123">Authorization</span></span>|<span data-ttu-id="e19dd-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e19dd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e19dd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e19dd-125">Accept</span></span>|<span data-ttu-id="e19dd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e19dd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e19dd-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e19dd-127">Request body</span></span>
<span data-ttu-id="e19dd-128">В тексте запроса добавьте представление объекта Усерекспериенцеаналитиксапфеалсосверсионперформанце в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e19dd-128">In the request body, supply a JSON representation for the userExperienceAnalyticsAppHealthOSVersionPerformance object.</span></span>

<span data-ttu-id="e19dd-129">В следующей таблице приведены свойства, необходимые при создании Усерекспериенцеаналитиксапфеалсосверсионперформанце.</span><span class="sxs-lookup"><span data-stu-id="e19dd-129">The following table shows the properties that are required when you create the userExperienceAnalyticsAppHealthOSVersionPerformance.</span></span>

|<span data-ttu-id="e19dd-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e19dd-130">Property</span></span>|<span data-ttu-id="e19dd-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e19dd-131">Type</span></span>|<span data-ttu-id="e19dd-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e19dd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e19dd-133">id</span><span class="sxs-lookup"><span data-stu-id="e19dd-133">id</span></span>|<span data-ttu-id="e19dd-134">String</span><span class="sxs-lookup"><span data-stu-id="e19dd-134">String</span></span>|<span data-ttu-id="e19dd-135">Уникальный идентификатор объекта производительности для версии службы аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="e19dd-135">The unique identifier of the user experience analytics OS version performance object.</span></span>|
|<span data-ttu-id="e19dd-136">osVersion</span><span class="sxs-lookup"><span data-stu-id="e19dd-136">osVersion</span></span>|<span data-ttu-id="e19dd-137">String</span><span class="sxs-lookup"><span data-stu-id="e19dd-137">String</span></span>|<span data-ttu-id="e19dd-138">Версия ОС, установленная на устройстве.</span><span class="sxs-lookup"><span data-stu-id="e19dd-138">The OS version installed on the device.</span></span>|
|<span data-ttu-id="e19dd-139">осбуилднумбер</span><span class="sxs-lookup"><span data-stu-id="e19dd-139">osBuildNumber</span></span>|<span data-ttu-id="e19dd-140">String</span><span class="sxs-lookup"><span data-stu-id="e19dd-140">String</span></span>|<span data-ttu-id="e19dd-141">Номер сборки ОС, установленный на устройстве.</span><span class="sxs-lookup"><span data-stu-id="e19dd-141">The OS build number installed on the device.</span></span>|
|<span data-ttu-id="e19dd-142">активедевицекаунт</span><span class="sxs-lookup"><span data-stu-id="e19dd-142">activeDeviceCount</span></span>|<span data-ttu-id="e19dd-143">Int32</span><span class="sxs-lookup"><span data-stu-id="e19dd-143">Int32</span></span>|<span data-ttu-id="e19dd-144">Число активных устройств для версии ОС.</span><span class="sxs-lookup"><span data-stu-id="e19dd-144">The number of active devices for the OS version.</span></span> <span data-ttu-id="e19dd-145">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="e19dd-145">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="e19dd-146">меантиметофаилуреинминутес</span><span class="sxs-lookup"><span data-stu-id="e19dd-146">meanTimeToFailureInMinutes</span></span>|<span data-ttu-id="e19dd-147">Int32</span><span class="sxs-lookup"><span data-stu-id="e19dd-147">Int32</span></span>|<span data-ttu-id="e19dd-148">Среднее время до сбоя для версии ОС в минутах.</span><span class="sxs-lookup"><span data-stu-id="e19dd-148">The mean time to failure for the OS version in minutes.</span></span> <span data-ttu-id="e19dd-149">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="e19dd-149">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="e19dd-150">осверсионапфеалсскоре</span><span class="sxs-lookup"><span data-stu-id="e19dd-150">osVersionAppHealthScore</span></span>|<span data-ttu-id="e19dd-151">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="e19dd-151">Double</span></span>|<span data-ttu-id="e19dd-152">Показатель работоспособности приложения для версии ОС.</span><span class="sxs-lookup"><span data-stu-id="e19dd-152">The app health score of the OS version.</span></span> <span data-ttu-id="e19dd-153">Допустимые значения — 1 79769313486232e308 E + 308 — 1 79769313486232e308 E + 308</span><span class="sxs-lookup"><span data-stu-id="e19dd-153">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="e19dd-154">осверсионапфеалсстатус</span><span class="sxs-lookup"><span data-stu-id="e19dd-154">osVersionAppHealthStatus</span></span>|<span data-ttu-id="e19dd-155">String</span><span class="sxs-lookup"><span data-stu-id="e19dd-155">String</span></span>|<span data-ttu-id="e19dd-156">Общее состояние работоспособности приложения для версии ОС.</span><span class="sxs-lookup"><span data-stu-id="e19dd-156">The overall app health status of the OS version.</span></span>|



## <a name="response"></a><span data-ttu-id="e19dd-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="e19dd-157">Response</span></span>
<span data-ttu-id="e19dd-158">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [усерекспериенцеаналитиксапфеалсосверсионперформанце](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e19dd-158">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsAppHealthOSVersionPerformance](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e19dd-159">Пример</span><span class="sxs-lookup"><span data-stu-id="e19dd-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="e19dd-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="e19dd-160">Request</span></span>
<span data-ttu-id="e19dd-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e19dd-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthOSVersionPerformance
Content-type: application/json
Content-length: 357

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthOSVersionPerformance",
  "osVersion": "Os Version value",
  "osBuildNumber": "Os Build Number value",
  "activeDeviceCount": 1,
  "meanTimeToFailureInMinutes": 10,
  "osVersionAppHealthScore": 7.666666666666667,
  "osVersionAppHealthStatus": "Os Version App Health Status value"
}
```

### <a name="response"></a><span data-ttu-id="e19dd-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="e19dd-162">Response</span></span>
<span data-ttu-id="e19dd-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e19dd-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 406

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthOSVersionPerformance",
  "id": "7c28e16b-e16b-7c28-6be1-287c6be1287c",
  "osVersion": "Os Version value",
  "osBuildNumber": "Os Build Number value",
  "activeDeviceCount": 1,
  "meanTimeToFailureInMinutes": 10,
  "osVersionAppHealthScore": 7.666666666666667,
  "osVersionAppHealthStatus": "Os Version App Health Status value"
}
```






