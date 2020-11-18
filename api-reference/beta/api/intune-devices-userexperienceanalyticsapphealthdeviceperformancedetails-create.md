---
title: Создание Усерекспериенцеаналитиксапфеалсдевицеперформанцедетаилс
description: Создание нового объекта Усерекспериенцеаналитиксапфеалсдевицеперформанцедетаилс.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4712d12d380b23a21efd044cc2bc8eb0e2b6d9e7
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49202802"
---
# <a name="create-userexperienceanalyticsapphealthdeviceperformancedetails"></a><span data-ttu-id="de3eb-103">Создание Усерекспериенцеаналитиксапфеалсдевицеперформанцедетаилс</span><span class="sxs-lookup"><span data-stu-id="de3eb-103">Create userExperienceAnalyticsAppHealthDevicePerformanceDetails</span></span>

<span data-ttu-id="de3eb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de3eb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="de3eb-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de3eb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="de3eb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="de3eb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de3eb-107">Создание нового объекта [усерекспериенцеаналитиксапфеалсдевицеперформанцедетаилс](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md) .</span><span class="sxs-lookup"><span data-stu-id="de3eb-107">Create a new [userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="de3eb-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="de3eb-108">Prerequisites</span></span>
<span data-ttu-id="de3eb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de3eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de3eb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="de3eb-111">Permission type</span></span>|<span data-ttu-id="de3eb-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="de3eb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="de3eb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="de3eb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="de3eb-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de3eb-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="de3eb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="de3eb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de3eb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de3eb-116">Not supported.</span></span>|
|<span data-ttu-id="de3eb-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="de3eb-117">Application</span></span>|<span data-ttu-id="de3eb-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de3eb-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="de3eb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="de3eb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsAppHealthDevicePerformanceDetails
```

## <a name="request-headers"></a><span data-ttu-id="de3eb-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="de3eb-120">Request headers</span></span>
|<span data-ttu-id="de3eb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="de3eb-121">Header</span></span>|<span data-ttu-id="de3eb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="de3eb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="de3eb-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="de3eb-123">Authorization</span></span>|<span data-ttu-id="de3eb-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="de3eb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="de3eb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="de3eb-125">Accept</span></span>|<span data-ttu-id="de3eb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="de3eb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="de3eb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="de3eb-127">Request body</span></span>
<span data-ttu-id="de3eb-128">В тексте запроса добавьте представление объекта Усерекспериенцеаналитиксапфеалсдевицеперформанцедетаилс в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="de3eb-128">In the request body, supply a JSON representation for the userExperienceAnalyticsAppHealthDevicePerformanceDetails object.</span></span>

<span data-ttu-id="de3eb-129">В следующей таблице приведены свойства, необходимые при создании Усерекспериенцеаналитиксапфеалсдевицеперформанцедетаилс.</span><span class="sxs-lookup"><span data-stu-id="de3eb-129">The following table shows the properties that are required when you create the userExperienceAnalyticsAppHealthDevicePerformanceDetails.</span></span>

|<span data-ttu-id="de3eb-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="de3eb-130">Property</span></span>|<span data-ttu-id="de3eb-131">Тип</span><span class="sxs-lookup"><span data-stu-id="de3eb-131">Type</span></span>|<span data-ttu-id="de3eb-132">Описание</span><span class="sxs-lookup"><span data-stu-id="de3eb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de3eb-133">id</span><span class="sxs-lookup"><span data-stu-id="de3eb-133">id</span></span>|<span data-ttu-id="de3eb-134">String</span><span class="sxs-lookup"><span data-stu-id="de3eb-134">String</span></span>|<span data-ttu-id="de3eb-135">Уникальный идентификатор объекта производительности устройства аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="de3eb-135">The unique identifier of the user experience analytics device performance object.</span></span>|
|<span data-ttu-id="de3eb-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="de3eb-136">eventDateTime</span></span>|<span data-ttu-id="de3eb-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de3eb-137">DateTimeOffset</span></span>|<span data-ttu-id="de3eb-138">Время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="de3eb-138">The time the event occurred.</span></span>|
|<span data-ttu-id="de3eb-139">eventType</span><span class="sxs-lookup"><span data-stu-id="de3eb-139">eventType</span></span>|<span data-ttu-id="de3eb-140">String</span><span class="sxs-lookup"><span data-stu-id="de3eb-140">String</span></span>|<span data-ttu-id="de3eb-141">Тип события.</span><span class="sxs-lookup"><span data-stu-id="de3eb-141">The type of the event.</span></span>|
|<span data-ttu-id="de3eb-142">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="de3eb-142">appDisplayName</span></span>|<span data-ttu-id="de3eb-143">String</span><span class="sxs-lookup"><span data-stu-id="de3eb-143">String</span></span>|<span data-ttu-id="de3eb-144">Понятное имя приложения, для которого произошло событие.</span><span class="sxs-lookup"><span data-stu-id="de3eb-144">The friendly name of the application for which the event occurred.</span></span>|
|<span data-ttu-id="de3eb-145">deviceId</span><span class="sxs-lookup"><span data-stu-id="de3eb-145">deviceId</span></span>|<span data-ttu-id="de3eb-146">String</span><span class="sxs-lookup"><span data-stu-id="de3eb-146">String</span></span>|<span data-ttu-id="de3eb-147">Идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="de3eb-147">The id of the device.</span></span>|
|<span data-ttu-id="de3eb-148">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="de3eb-148">deviceDisplayName</span></span>|<span data-ttu-id="de3eb-149">String</span><span class="sxs-lookup"><span data-stu-id="de3eb-149">String</span></span>|<span data-ttu-id="de3eb-150">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="de3eb-150">The name of the device.</span></span>|



## <a name="response"></a><span data-ttu-id="de3eb-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="de3eb-151">Response</span></span>
<span data-ttu-id="de3eb-152">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [усерекспериенцеаналитиксапфеалсдевицеперформанцедетаилс](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="de3eb-152">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de3eb-153">Пример</span><span class="sxs-lookup"><span data-stu-id="de3eb-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="de3eb-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="de3eb-154">Request</span></span>
<span data-ttu-id="de3eb-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="de3eb-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthDevicePerformanceDetails
Content-type: application/json
Content-length: 325

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthDevicePerformanceDetails",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "eventType": "Event Type value",
  "appDisplayName": "App Display Name value",
  "deviceId": "Device Id value",
  "deviceDisplayName": "Device Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="de3eb-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="de3eb-156">Response</span></span>
<span data-ttu-id="de3eb-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="de3eb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 374

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthDevicePerformanceDetails",
  "id": "bc8c5273-5273-bc8c-7352-8cbc73528cbc",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "eventType": "Event Type value",
  "appDisplayName": "App Display Name value",
  "deviceId": "Device Id value",
  "deviceDisplayName": "Device Display Name value"
}
```




