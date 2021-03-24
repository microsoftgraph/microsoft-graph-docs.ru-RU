---
title: Создание userExperienceAnalyticsAppHealthOSVersionPerformance
description: Создание нового объекта userExperienceAnalyticsAppHealthOSVersionPerformance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 80ae02ef79f06808a83997c494862d769e82bce2
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51136001"
---
# <a name="create-userexperienceanalyticsapphealthosversionperformance"></a><span data-ttu-id="9d67e-103">Создание userExperienceAnalyticsAppHealthOSVersionPerformance</span><span class="sxs-lookup"><span data-stu-id="9d67e-103">Create userExperienceAnalyticsAppHealthOSVersionPerformance</span></span>

<span data-ttu-id="9d67e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d67e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9d67e-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d67e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9d67e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9d67e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d67e-107">Создание нового [объекта userExperienceAnalyticsAppHealthOSVersionPerformance.](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md)</span><span class="sxs-lookup"><span data-stu-id="9d67e-107">Create a new [userExperienceAnalyticsAppHealthOSVersionPerformance](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9d67e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9d67e-108">Prerequisites</span></span>
<span data-ttu-id="9d67e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d67e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d67e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9d67e-111">Permission type</span></span>|<span data-ttu-id="9d67e-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9d67e-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9d67e-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9d67e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9d67e-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d67e-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="9d67e-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9d67e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9d67e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d67e-116">Not supported.</span></span>|
|<span data-ttu-id="9d67e-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="9d67e-117">Application</span></span>|<span data-ttu-id="9d67e-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d67e-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9d67e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9d67e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsAppHealthOSVersionPerformance
```

## <a name="request-headers"></a><span data-ttu-id="9d67e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9d67e-120">Request headers</span></span>
|<span data-ttu-id="9d67e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9d67e-121">Header</span></span>|<span data-ttu-id="9d67e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9d67e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9d67e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d67e-123">Authorization</span></span>|<span data-ttu-id="9d67e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9d67e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9d67e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9d67e-125">Accept</span></span>|<span data-ttu-id="9d67e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9d67e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d67e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9d67e-127">Request body</span></span>
<span data-ttu-id="9d67e-128">В теле запроса поставляем представление JSON для объекта userExperienceAnalyticsAppHealthOSVersionPerformance.</span><span class="sxs-lookup"><span data-stu-id="9d67e-128">In the request body, supply a JSON representation for the userExperienceAnalyticsAppHealthOSVersionPerformance object.</span></span>

<span data-ttu-id="9d67e-129">В следующей таблице показаны свойства, необходимые при создании userExperienceAnalyticsAppHealthOSVersionPerformance.</span><span class="sxs-lookup"><span data-stu-id="9d67e-129">The following table shows the properties that are required when you create the userExperienceAnalyticsAppHealthOSVersionPerformance.</span></span>

|<span data-ttu-id="9d67e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9d67e-130">Property</span></span>|<span data-ttu-id="9d67e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9d67e-131">Type</span></span>|<span data-ttu-id="9d67e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9d67e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d67e-133">id</span><span class="sxs-lookup"><span data-stu-id="9d67e-133">id</span></span>|<span data-ttu-id="9d67e-134">Строка</span><span class="sxs-lookup"><span data-stu-id="9d67e-134">String</span></span>|<span data-ttu-id="9d67e-135">Уникальный идентификатор объекта производительности версии оси для пользовательского интерфейса аналитики оси.</span><span class="sxs-lookup"><span data-stu-id="9d67e-135">The unique identifier of the user experience analytics OS version performance object.</span></span>|
|<span data-ttu-id="9d67e-136">osVersion</span><span class="sxs-lookup"><span data-stu-id="9d67e-136">osVersion</span></span>|<span data-ttu-id="9d67e-137">String</span><span class="sxs-lookup"><span data-stu-id="9d67e-137">String</span></span>|<span data-ttu-id="9d67e-138">Версия ОС, установленная на устройстве.</span><span class="sxs-lookup"><span data-stu-id="9d67e-138">The OS version installed on the device.</span></span>|
|<span data-ttu-id="9d67e-139">osBuildNumber</span><span class="sxs-lookup"><span data-stu-id="9d67e-139">osBuildNumber</span></span>|<span data-ttu-id="9d67e-140">Строка</span><span class="sxs-lookup"><span data-stu-id="9d67e-140">String</span></span>|<span data-ttu-id="9d67e-141">Номер сборки ОС, установленный на устройстве.</span><span class="sxs-lookup"><span data-stu-id="9d67e-141">The OS build number installed on the device.</span></span>|
|<span data-ttu-id="9d67e-142">activeDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9d67e-142">activeDeviceCount</span></span>|<span data-ttu-id="9d67e-143">Int32</span><span class="sxs-lookup"><span data-stu-id="9d67e-143">Int32</span></span>|<span data-ttu-id="9d67e-144">Количество активных устройств для версии ОС.</span><span class="sxs-lookup"><span data-stu-id="9d67e-144">The number of active devices for the OS version.</span></span> <span data-ttu-id="9d67e-145">Допустимые значения -2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="9d67e-145">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="9d67e-146">meanTimeToFailureInMinutes</span><span class="sxs-lookup"><span data-stu-id="9d67e-146">meanTimeToFailureInMinutes</span></span>|<span data-ttu-id="9d67e-147">Int32</span><span class="sxs-lookup"><span data-stu-id="9d67e-147">Int32</span></span>|<span data-ttu-id="9d67e-148">Время сбоя для версии ОС в минутах.</span><span class="sxs-lookup"><span data-stu-id="9d67e-148">The mean time to failure for the OS version in minutes.</span></span> <span data-ttu-id="9d67e-149">Допустимые значения -2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="9d67e-149">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="9d67e-150">osVersionAppHealthScore</span><span class="sxs-lookup"><span data-stu-id="9d67e-150">osVersionAppHealthScore</span></span>|<span data-ttu-id="9d67e-151">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="9d67e-151">Double</span></span>|<span data-ttu-id="9d67e-152">Оценка состояния здоровья приложения в версии ОС.</span><span class="sxs-lookup"><span data-stu-id="9d67e-152">The app health score of the OS version.</span></span> <span data-ttu-id="9d67e-153">Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308</span><span class="sxs-lookup"><span data-stu-id="9d67e-153">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="9d67e-154">osVersionAppHealthStatus</span><span class="sxs-lookup"><span data-stu-id="9d67e-154">osVersionAppHealthStatus</span></span>|<span data-ttu-id="9d67e-155">Строка</span><span class="sxs-lookup"><span data-stu-id="9d67e-155">String</span></span>|<span data-ttu-id="9d67e-156">Общее состояние состояния здоровья приложения в версии ОС.</span><span class="sxs-lookup"><span data-stu-id="9d67e-156">The overall app health status of the OS version.</span></span>|



## <a name="response"></a><span data-ttu-id="9d67e-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="9d67e-157">Response</span></span>
<span data-ttu-id="9d67e-158">В случае успеха этот метод возвращает код отклика и объект `201 Created` [userExperienceAnalyticsAppHealthOSVersionPerformance](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="9d67e-158">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsAppHealthOSVersionPerformance](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d67e-159">Пример</span><span class="sxs-lookup"><span data-stu-id="9d67e-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="9d67e-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="9d67e-160">Request</span></span>
<span data-ttu-id="9d67e-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9d67e-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9d67e-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="9d67e-162">Response</span></span>
<span data-ttu-id="9d67e-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9d67e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




