---
title: Обновление Усерекспериенцеаналитиксапфеалсдевицемоделперформанце
description: Обновление свойств объекта Усерекспериенцеаналитиксапфеалсдевицемоделперформанце.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 43c1cca17b1718debae367a950a3e90102b355c1
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49202901"
---
# <a name="update-userexperienceanalyticsapphealthdevicemodelperformance"></a><span data-ttu-id="123c2-103">Обновление Усерекспериенцеаналитиксапфеалсдевицемоделперформанце</span><span class="sxs-lookup"><span data-stu-id="123c2-103">Update userExperienceAnalyticsAppHealthDeviceModelPerformance</span></span>

<span data-ttu-id="123c2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="123c2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="123c2-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="123c2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="123c2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="123c2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="123c2-107">Обновление свойств объекта [усерекспериенцеаналитиксапфеалсдевицемоделперформанце](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) .</span><span class="sxs-lookup"><span data-stu-id="123c2-107">Update the properties of a [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="123c2-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="123c2-108">Prerequisites</span></span>
<span data-ttu-id="123c2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="123c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="123c2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="123c2-111">Permission type</span></span>|<span data-ttu-id="123c2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="123c2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="123c2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="123c2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="123c2-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="123c2-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="123c2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="123c2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="123c2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="123c2-116">Not supported.</span></span>|
|<span data-ttu-id="123c2-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="123c2-117">Application</span></span>|<span data-ttu-id="123c2-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="123c2-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="123c2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="123c2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsAppHealthDeviceModelPerformance/{userExperienceAnalyticsAppHealthDeviceModelPerformanceId}
```

## <a name="request-headers"></a><span data-ttu-id="123c2-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="123c2-120">Request headers</span></span>
|<span data-ttu-id="123c2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="123c2-121">Header</span></span>|<span data-ttu-id="123c2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="123c2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="123c2-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="123c2-123">Authorization</span></span>|<span data-ttu-id="123c2-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="123c2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="123c2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="123c2-125">Accept</span></span>|<span data-ttu-id="123c2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="123c2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="123c2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="123c2-127">Request body</span></span>
<span data-ttu-id="123c2-128">В тексте запроса добавьте представление объекта [усерекспериенцеаналитиксапфеалсдевицемоделперформанце](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="123c2-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) object.</span></span>

<span data-ttu-id="123c2-129">В следующей таблице приведены свойства, необходимые при создании [усерекспериенцеаналитиксапфеалсдевицемоделперформанце](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md).</span><span class="sxs-lookup"><span data-stu-id="123c2-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md).</span></span>

|<span data-ttu-id="123c2-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="123c2-130">Property</span></span>|<span data-ttu-id="123c2-131">Тип</span><span class="sxs-lookup"><span data-stu-id="123c2-131">Type</span></span>|<span data-ttu-id="123c2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="123c2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="123c2-133">id</span><span class="sxs-lookup"><span data-stu-id="123c2-133">id</span></span>|<span data-ttu-id="123c2-134">String</span><span class="sxs-lookup"><span data-stu-id="123c2-134">String</span></span>|<span data-ttu-id="123c2-135">Уникальный идентификатор объекта производительности модели устройства Analytics User Experience.</span><span class="sxs-lookup"><span data-stu-id="123c2-135">The unique identifier of the user experience analytics device model performance object.</span></span>|
|<span data-ttu-id="123c2-136">deviceModel</span><span class="sxs-lookup"><span data-stu-id="123c2-136">deviceModel</span></span>|<span data-ttu-id="123c2-137">String</span><span class="sxs-lookup"><span data-stu-id="123c2-137">String</span></span>|<span data-ttu-id="123c2-138">Имя модели устройства.</span><span class="sxs-lookup"><span data-stu-id="123c2-138">The model name of the device.</span></span>|
|<span data-ttu-id="123c2-139">девицемануфактурер</span><span class="sxs-lookup"><span data-stu-id="123c2-139">deviceManufacturer</span></span>|<span data-ttu-id="123c2-140">String</span><span class="sxs-lookup"><span data-stu-id="123c2-140">String</span></span>|<span data-ttu-id="123c2-141">Название изготовителя устройства.</span><span class="sxs-lookup"><span data-stu-id="123c2-141">The manufacturer name of the device.</span></span>|
|<span data-ttu-id="123c2-142">активедевицекаунт</span><span class="sxs-lookup"><span data-stu-id="123c2-142">activeDeviceCount</span></span>|<span data-ttu-id="123c2-143">Int32</span><span class="sxs-lookup"><span data-stu-id="123c2-143">Int32</span></span>|<span data-ttu-id="123c2-144">Количество активных устройств для модели.</span><span class="sxs-lookup"><span data-stu-id="123c2-144">The number of active devices for the model.</span></span> <span data-ttu-id="123c2-145">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="123c2-145">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="123c2-146">меантиметофаилуреинминутес</span><span class="sxs-lookup"><span data-stu-id="123c2-146">meanTimeToFailureInMinutes</span></span>|<span data-ttu-id="123c2-147">Int32</span><span class="sxs-lookup"><span data-stu-id="123c2-147">Int32</span></span>|<span data-ttu-id="123c2-148">Среднее время до сбоя устройства модели в минутах.</span><span class="sxs-lookup"><span data-stu-id="123c2-148">The mean time to failure for the model device in minutes.</span></span> <span data-ttu-id="123c2-149">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="123c2-149">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="123c2-150">моделапфеалсскоре</span><span class="sxs-lookup"><span data-stu-id="123c2-150">modelAppHealthScore</span></span>|<span data-ttu-id="123c2-151">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="123c2-151">Double</span></span>|<span data-ttu-id="123c2-152">Показатель работоспособности приложения модели устройства.</span><span class="sxs-lookup"><span data-stu-id="123c2-152">The app health score of the device model.</span></span> <span data-ttu-id="123c2-153">Допустимые значения — 1 79769313486232e308 E + 308 — 1 79769313486232e308 E + 308</span><span class="sxs-lookup"><span data-stu-id="123c2-153">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="123c2-154">моделапфеалсстатус</span><span class="sxs-lookup"><span data-stu-id="123c2-154">modelAppHealthStatus</span></span>|<span data-ttu-id="123c2-155">String</span><span class="sxs-lookup"><span data-stu-id="123c2-155">String</span></span>|<span data-ttu-id="123c2-156">Общее состояние работоспособности приложения модели устройства.</span><span class="sxs-lookup"><span data-stu-id="123c2-156">The overall app health status of the device model.</span></span>|



## <a name="response"></a><span data-ttu-id="123c2-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="123c2-157">Response</span></span>
<span data-ttu-id="123c2-158">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [усерекспериенцеаналитиксапфеалсдевицемоделперформанце](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="123c2-158">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="123c2-159">Пример</span><span class="sxs-lookup"><span data-stu-id="123c2-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="123c2-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="123c2-160">Request</span></span>
<span data-ttu-id="123c2-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="123c2-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthDeviceModelPerformance/{userExperienceAnalyticsAppHealthDeviceModelPerformanceId}
Content-type: application/json
Content-length: 359

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthDeviceModelPerformance",
  "deviceModel": "Device Model value",
  "deviceManufacturer": "Device Manufacturer value",
  "activeDeviceCount": 1,
  "meanTimeToFailureInMinutes": 10,
  "modelAppHealthScore": 6.333333333333333,
  "modelAppHealthStatus": "Model App Health Status value"
}
```

### <a name="response"></a><span data-ttu-id="123c2-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="123c2-162">Response</span></span>
<span data-ttu-id="123c2-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="123c2-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 408

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthDeviceModelPerformance",
  "id": "4daddc60-dc60-4dad-60dc-ad4d60dcad4d",
  "deviceModel": "Device Model value",
  "deviceManufacturer": "Device Manufacturer value",
  "activeDeviceCount": 1,
  "meanTimeToFailureInMinutes": 10,
  "modelAppHealthScore": 6.333333333333333,
  "modelAppHealthStatus": "Model App Health Status value"
}
```




