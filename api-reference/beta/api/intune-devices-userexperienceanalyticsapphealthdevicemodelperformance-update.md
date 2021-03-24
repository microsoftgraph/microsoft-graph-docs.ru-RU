---
title: Обновление userExperienceAnalyticsAppHealthDeviceModelPerformance
description: Обновление свойств объекта userExperienceAnalyticsAppHealthDeviceModelPerformance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 26667c68a45158a29c991dc91be28bce0cf13fd9
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51136162"
---
# <a name="update-userexperienceanalyticsapphealthdevicemodelperformance"></a><span data-ttu-id="7b3b0-103">Обновление userExperienceAnalyticsAppHealthDeviceModelPerformance</span><span class="sxs-lookup"><span data-stu-id="7b3b0-103">Update userExperienceAnalyticsAppHealthDeviceModelPerformance</span></span>

<span data-ttu-id="7b3b0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b3b0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7b3b0-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b3b0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7b3b0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7b3b0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7b3b0-107">Обновление свойств объекта [userExperienceAnalyticsAppHealthDeviceModelPerformance.](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md)</span><span class="sxs-lookup"><span data-stu-id="7b3b0-107">Update the properties of a [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7b3b0-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7b3b0-108">Prerequisites</span></span>
<span data-ttu-id="7b3b0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b3b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b3b0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7b3b0-111">Permission type</span></span>|<span data-ttu-id="7b3b0-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7b3b0-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7b3b0-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7b3b0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7b3b0-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b3b0-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="7b3b0-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7b3b0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7b3b0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b3b0-116">Not supported.</span></span>|
|<span data-ttu-id="7b3b0-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="7b3b0-117">Application</span></span>|<span data-ttu-id="7b3b0-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b3b0-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7b3b0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7b3b0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsAppHealthDeviceModelPerformance/{userExperienceAnalyticsAppHealthDeviceModelPerformanceId}
```

## <a name="request-headers"></a><span data-ttu-id="7b3b0-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7b3b0-120">Request headers</span></span>
|<span data-ttu-id="7b3b0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7b3b0-121">Header</span></span>|<span data-ttu-id="7b3b0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7b3b0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7b3b0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b3b0-123">Authorization</span></span>|<span data-ttu-id="7b3b0-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7b3b0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7b3b0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7b3b0-125">Accept</span></span>|<span data-ttu-id="7b3b0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7b3b0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b3b0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7b3b0-127">Request body</span></span>
<span data-ttu-id="7b3b0-128">В теле запроса поставляем представление JSON для [объекта userExperienceAnalyticsAppHealthDeviceModelPerformance.](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md)</span><span class="sxs-lookup"><span data-stu-id="7b3b0-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) object.</span></span>

<span data-ttu-id="7b3b0-129">В следующей таблице показаны свойства, необходимые при создании [пользователяExperienceAnalyticsAppHealthDeviceModelPerformance.](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md)</span><span class="sxs-lookup"><span data-stu-id="7b3b0-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md).</span></span>

|<span data-ttu-id="7b3b0-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7b3b0-130">Property</span></span>|<span data-ttu-id="7b3b0-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7b3b0-131">Type</span></span>|<span data-ttu-id="7b3b0-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7b3b0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b3b0-133">id</span><span class="sxs-lookup"><span data-stu-id="7b3b0-133">id</span></span>|<span data-ttu-id="7b3b0-134">Строка</span><span class="sxs-lookup"><span data-stu-id="7b3b0-134">String</span></span>|<span data-ttu-id="7b3b0-135">Уникальный идентификатор объекта производительности модели пользовательского интерфейса для аналитики устройств.</span><span class="sxs-lookup"><span data-stu-id="7b3b0-135">The unique identifier of the user experience analytics device model performance object.</span></span>|
|<span data-ttu-id="7b3b0-136">deviceModel</span><span class="sxs-lookup"><span data-stu-id="7b3b0-136">deviceModel</span></span>|<span data-ttu-id="7b3b0-137">String</span><span class="sxs-lookup"><span data-stu-id="7b3b0-137">String</span></span>|<span data-ttu-id="7b3b0-138">Имя модели устройства.</span><span class="sxs-lookup"><span data-stu-id="7b3b0-138">The model name of the device.</span></span>|
|<span data-ttu-id="7b3b0-139">deviceManufacturer</span><span class="sxs-lookup"><span data-stu-id="7b3b0-139">deviceManufacturer</span></span>|<span data-ttu-id="7b3b0-140">Строка</span><span class="sxs-lookup"><span data-stu-id="7b3b0-140">String</span></span>|<span data-ttu-id="7b3b0-141">Имя производителя устройства.</span><span class="sxs-lookup"><span data-stu-id="7b3b0-141">The manufacturer name of the device.</span></span>|
|<span data-ttu-id="7b3b0-142">activeDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7b3b0-142">activeDeviceCount</span></span>|<span data-ttu-id="7b3b0-143">Int32</span><span class="sxs-lookup"><span data-stu-id="7b3b0-143">Int32</span></span>|<span data-ttu-id="7b3b0-144">Количество активных устройств для модели.</span><span class="sxs-lookup"><span data-stu-id="7b3b0-144">The number of active devices for the model.</span></span> <span data-ttu-id="7b3b0-145">Допустимые значения -2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="7b3b0-145">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="7b3b0-146">meanTimeToFailureInMinutes</span><span class="sxs-lookup"><span data-stu-id="7b3b0-146">meanTimeToFailureInMinutes</span></span>|<span data-ttu-id="7b3b0-147">Int32</span><span class="sxs-lookup"><span data-stu-id="7b3b0-147">Int32</span></span>|<span data-ttu-id="7b3b0-148">Время сбоя для устройства модели в минутах.</span><span class="sxs-lookup"><span data-stu-id="7b3b0-148">The mean time to failure for the model device in minutes.</span></span> <span data-ttu-id="7b3b0-149">Допустимые значения -2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="7b3b0-149">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="7b3b0-150">modelAppHealthScore</span><span class="sxs-lookup"><span data-stu-id="7b3b0-150">modelAppHealthScore</span></span>|<span data-ttu-id="7b3b0-151">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="7b3b0-151">Double</span></span>|<span data-ttu-id="7b3b0-152">Оценка состояния здоровья приложения модели устройства.</span><span class="sxs-lookup"><span data-stu-id="7b3b0-152">The app health score of the device model.</span></span> <span data-ttu-id="7b3b0-153">Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308</span><span class="sxs-lookup"><span data-stu-id="7b3b0-153">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="7b3b0-154">modelAppHealthStatus</span><span class="sxs-lookup"><span data-stu-id="7b3b0-154">modelAppHealthStatus</span></span>|<span data-ttu-id="7b3b0-155">Строка</span><span class="sxs-lookup"><span data-stu-id="7b3b0-155">String</span></span>|<span data-ttu-id="7b3b0-156">Общее состояние состояния здоровья приложения модели устройства.</span><span class="sxs-lookup"><span data-stu-id="7b3b0-156">The overall app health status of the device model.</span></span>|



## <a name="response"></a><span data-ttu-id="7b3b0-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="7b3b0-157">Response</span></span>
<span data-ttu-id="7b3b0-158">В случае успеха этот метод возвращает код ответа и обновленный объект `200 OK` [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="7b3b0-158">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b3b0-159">Пример</span><span class="sxs-lookup"><span data-stu-id="7b3b0-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="7b3b0-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="7b3b0-160">Request</span></span>
<span data-ttu-id="7b3b0-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7b3b0-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7b3b0-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="7b3b0-162">Response</span></span>
<span data-ttu-id="7b3b0-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7b3b0-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




