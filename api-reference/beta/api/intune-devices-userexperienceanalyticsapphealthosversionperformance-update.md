---
title: Обновление userExperienceAnalyticsAppHealthOSVersionPerformance
description: Обновление свойств объекта userExperienceAnalyticsAppHealthOSVersionPerformance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 67fc4fbe6128842db99fb70a2198da21bfd30714
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51157949"
---
# <a name="update-userexperienceanalyticsapphealthosversionperformance"></a><span data-ttu-id="df004-103">Обновление userExperienceAnalyticsAppHealthOSVersionPerformance</span><span class="sxs-lookup"><span data-stu-id="df004-103">Update userExperienceAnalyticsAppHealthOSVersionPerformance</span></span>

<span data-ttu-id="df004-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df004-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="df004-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="df004-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="df004-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="df004-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df004-107">Обновление свойств объекта [userExperienceAnalyticsAppHealthOSVersionPerformance.](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md)</span><span class="sxs-lookup"><span data-stu-id="df004-107">Update the properties of a [userExperienceAnalyticsAppHealthOSVersionPerformance](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="df004-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="df004-108">Prerequisites</span></span>
<span data-ttu-id="df004-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df004-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df004-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="df004-111">Permission type</span></span>|<span data-ttu-id="df004-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="df004-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="df004-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="df004-113">Delegated (work or school account)</span></span>|<span data-ttu-id="df004-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df004-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="df004-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="df004-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df004-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="df004-116">Not supported.</span></span>|
|<span data-ttu-id="df004-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="df004-117">Application</span></span>|<span data-ttu-id="df004-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df004-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="df004-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="df004-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsAppHealthOSVersionPerformance/{userExperienceAnalyticsAppHealthOSVersionPerformanceId}
```

## <a name="request-headers"></a><span data-ttu-id="df004-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="df004-120">Request headers</span></span>
|<span data-ttu-id="df004-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="df004-121">Header</span></span>|<span data-ttu-id="df004-122">Значение</span><span class="sxs-lookup"><span data-stu-id="df004-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="df004-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="df004-123">Authorization</span></span>|<span data-ttu-id="df004-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="df004-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="df004-125">Accept</span><span class="sxs-lookup"><span data-stu-id="df004-125">Accept</span></span>|<span data-ttu-id="df004-126">application/json</span><span class="sxs-lookup"><span data-stu-id="df004-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="df004-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="df004-127">Request body</span></span>
<span data-ttu-id="df004-128">В теле запроса поставляем представление JSON для [объекта userExperienceAnalyticsAppHealthOSVersionPerformance.](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md)</span><span class="sxs-lookup"><span data-stu-id="df004-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsAppHealthOSVersionPerformance](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md) object.</span></span>

<span data-ttu-id="df004-129">В следующей таблице показаны свойства, необходимые при создании [userExperienceAnalyticsAppHealthOSVersionPerformance.](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md)</span><span class="sxs-lookup"><span data-stu-id="df004-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsAppHealthOSVersionPerformance](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md).</span></span>

|<span data-ttu-id="df004-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="df004-130">Property</span></span>|<span data-ttu-id="df004-131">Тип</span><span class="sxs-lookup"><span data-stu-id="df004-131">Type</span></span>|<span data-ttu-id="df004-132">Описание</span><span class="sxs-lookup"><span data-stu-id="df004-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df004-133">id</span><span class="sxs-lookup"><span data-stu-id="df004-133">id</span></span>|<span data-ttu-id="df004-134">Строка</span><span class="sxs-lookup"><span data-stu-id="df004-134">String</span></span>|<span data-ttu-id="df004-135">Уникальный идентификатор объекта производительности версии оси для пользовательского интерфейса аналитики оси.</span><span class="sxs-lookup"><span data-stu-id="df004-135">The unique identifier of the user experience analytics OS version performance object.</span></span>|
|<span data-ttu-id="df004-136">osVersion</span><span class="sxs-lookup"><span data-stu-id="df004-136">osVersion</span></span>|<span data-ttu-id="df004-137">String</span><span class="sxs-lookup"><span data-stu-id="df004-137">String</span></span>|<span data-ttu-id="df004-138">Версия ОС, установленная на устройстве.</span><span class="sxs-lookup"><span data-stu-id="df004-138">The OS version installed on the device.</span></span>|
|<span data-ttu-id="df004-139">osBuildNumber</span><span class="sxs-lookup"><span data-stu-id="df004-139">osBuildNumber</span></span>|<span data-ttu-id="df004-140">Строка</span><span class="sxs-lookup"><span data-stu-id="df004-140">String</span></span>|<span data-ttu-id="df004-141">Номер сборки ОС, установленный на устройстве.</span><span class="sxs-lookup"><span data-stu-id="df004-141">The OS build number installed on the device.</span></span>|
|<span data-ttu-id="df004-142">activeDeviceCount</span><span class="sxs-lookup"><span data-stu-id="df004-142">activeDeviceCount</span></span>|<span data-ttu-id="df004-143">Int32</span><span class="sxs-lookup"><span data-stu-id="df004-143">Int32</span></span>|<span data-ttu-id="df004-144">Количество активных устройств для версии ОС.</span><span class="sxs-lookup"><span data-stu-id="df004-144">The number of active devices for the OS version.</span></span> <span data-ttu-id="df004-145">Допустимые значения -2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="df004-145">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="df004-146">meanTimeToFailureInMinutes</span><span class="sxs-lookup"><span data-stu-id="df004-146">meanTimeToFailureInMinutes</span></span>|<span data-ttu-id="df004-147">Int32</span><span class="sxs-lookup"><span data-stu-id="df004-147">Int32</span></span>|<span data-ttu-id="df004-148">Время сбоя для версии ОС в минутах.</span><span class="sxs-lookup"><span data-stu-id="df004-148">The mean time to failure for the OS version in minutes.</span></span> <span data-ttu-id="df004-149">Допустимые значения -2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="df004-149">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="df004-150">osVersionAppHealthScore</span><span class="sxs-lookup"><span data-stu-id="df004-150">osVersionAppHealthScore</span></span>|<span data-ttu-id="df004-151">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="df004-151">Double</span></span>|<span data-ttu-id="df004-152">Оценка состояния здоровья приложения в версии ОС.</span><span class="sxs-lookup"><span data-stu-id="df004-152">The app health score of the OS version.</span></span> <span data-ttu-id="df004-153">Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308</span><span class="sxs-lookup"><span data-stu-id="df004-153">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="df004-154">osVersionAppHealthStatus</span><span class="sxs-lookup"><span data-stu-id="df004-154">osVersionAppHealthStatus</span></span>|<span data-ttu-id="df004-155">Строка</span><span class="sxs-lookup"><span data-stu-id="df004-155">String</span></span>|<span data-ttu-id="df004-156">Общее состояние состояния здоровья приложения в версии ОС.</span><span class="sxs-lookup"><span data-stu-id="df004-156">The overall app health status of the OS version.</span></span>|



## <a name="response"></a><span data-ttu-id="df004-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="df004-157">Response</span></span>
<span data-ttu-id="df004-158">В случае успеха этот метод возвращает код ответа и обновленный объект `200 OK` [userExperienceAnalyticsAppHealthOSVersionPerformance](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="df004-158">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsAppHealthOSVersionPerformance](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df004-159">Пример</span><span class="sxs-lookup"><span data-stu-id="df004-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="df004-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="df004-160">Request</span></span>
<span data-ttu-id="df004-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="df004-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthOSVersionPerformance/{userExperienceAnalyticsAppHealthOSVersionPerformanceId}
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

### <a name="response"></a><span data-ttu-id="df004-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="df004-162">Response</span></span>
<span data-ttu-id="df004-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="df004-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




