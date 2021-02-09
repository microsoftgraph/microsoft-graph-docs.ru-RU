---
title: Обновление unmanagedDeviceDiscoveryTask
description: Обновление свойств объекта unmanagedDeviceDiscoveryTask.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f7908c6a79cba41312d4f8ac850c78d32076c21b
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160808"
---
# <a name="update-unmanageddevicediscoverytask"></a><span data-ttu-id="3b7ca-103">Обновление unmanagedDeviceDiscoveryTask</span><span class="sxs-lookup"><span data-stu-id="3b7ca-103">Update unmanagedDeviceDiscoveryTask</span></span>

<span data-ttu-id="3b7ca-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b7ca-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3b7ca-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b7ca-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3b7ca-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3b7ca-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b7ca-107">Обновление свойств объекта [unmanagedDeviceDiscoveryTask.](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md)</span><span class="sxs-lookup"><span data-stu-id="3b7ca-107">Update the properties of a [unmanagedDeviceDiscoveryTask](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3b7ca-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3b7ca-108">Prerequisites</span></span>
<span data-ttu-id="3b7ca-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b7ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b7ca-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3b7ca-111">Permission type</span></span>|<span data-ttu-id="3b7ca-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3b7ca-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b7ca-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3b7ca-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3b7ca-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b7ca-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3b7ca-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3b7ca-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b7ca-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b7ca-116">Not supported.</span></span>|
|<span data-ttu-id="3b7ca-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3b7ca-117">Application</span></span>|<span data-ttu-id="3b7ca-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b7ca-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b7ca-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3b7ca-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/deviceAppManagementTasks/{deviceAppManagementTaskId}
```

## <a name="request-headers"></a><span data-ttu-id="3b7ca-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3b7ca-120">Request headers</span></span>
|<span data-ttu-id="3b7ca-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3b7ca-121">Header</span></span>|<span data-ttu-id="3b7ca-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3b7ca-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3b7ca-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3b7ca-123">Authorization</span></span>|<span data-ttu-id="3b7ca-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3b7ca-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3b7ca-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3b7ca-125">Accept</span></span>|<span data-ttu-id="3b7ca-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3b7ca-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b7ca-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3b7ca-127">Request body</span></span>
<span data-ttu-id="3b7ca-128">В теле запроса укажу представление объекта [unmanagedDeviceDiscoveryTask](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="3b7ca-128">In the request body, supply a JSON representation for the [unmanagedDeviceDiscoveryTask](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md) object.</span></span>

<span data-ttu-id="3b7ca-129">В следующей таблице показаны свойства, необходимые при создании [объекта unmanagedDeviceDiscoveryTask.](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md)</span><span class="sxs-lookup"><span data-stu-id="3b7ca-129">The following table shows the properties that are required when you create the [unmanagedDeviceDiscoveryTask](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md).</span></span>

|<span data-ttu-id="3b7ca-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3b7ca-130">Property</span></span>|<span data-ttu-id="3b7ca-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3b7ca-131">Type</span></span>|<span data-ttu-id="3b7ca-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3b7ca-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b7ca-133">id</span><span class="sxs-lookup"><span data-stu-id="3b7ca-133">id</span></span>|<span data-ttu-id="3b7ca-134">String</span><span class="sxs-lookup"><span data-stu-id="3b7ca-134">String</span></span>|<span data-ttu-id="3b7ca-135">Ключ сущности.</span><span class="sxs-lookup"><span data-stu-id="3b7ca-135">The entity key.</span></span> <span data-ttu-id="3b7ca-136">Наследуется [от deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="3b7ca-136">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="3b7ca-137">displayName</span><span class="sxs-lookup"><span data-stu-id="3b7ca-137">displayName</span></span>|<span data-ttu-id="3b7ca-138">String</span><span class="sxs-lookup"><span data-stu-id="3b7ca-138">String</span></span>|<span data-ttu-id="3b7ca-139">Имя.</span><span class="sxs-lookup"><span data-stu-id="3b7ca-139">The name.</span></span> <span data-ttu-id="3b7ca-140">Наследуется [от deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="3b7ca-140">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="3b7ca-141">description</span><span class="sxs-lookup"><span data-stu-id="3b7ca-141">description</span></span>|<span data-ttu-id="3b7ca-142">String</span><span class="sxs-lookup"><span data-stu-id="3b7ca-142">String</span></span>|<span data-ttu-id="3b7ca-143">Описание.</span><span class="sxs-lookup"><span data-stu-id="3b7ca-143">The description.</span></span> <span data-ttu-id="3b7ca-144">Наследуется [от deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="3b7ca-144">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="3b7ca-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3b7ca-145">createdDateTime</span></span>|<span data-ttu-id="3b7ca-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b7ca-146">DateTimeOffset</span></span>|<span data-ttu-id="3b7ca-147">Дата создания.</span><span class="sxs-lookup"><span data-stu-id="3b7ca-147">The created date.</span></span> <span data-ttu-id="3b7ca-148">Наследуется [от deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="3b7ca-148">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="3b7ca-149">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="3b7ca-149">dueDateTime</span></span>|<span data-ttu-id="3b7ca-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b7ca-150">DateTimeOffset</span></span>|<span data-ttu-id="3b7ca-151">Дата окончания.</span><span class="sxs-lookup"><span data-stu-id="3b7ca-151">The due date.</span></span> <span data-ttu-id="3b7ca-152">Наследуется [от deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="3b7ca-152">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="3b7ca-153">category</span><span class="sxs-lookup"><span data-stu-id="3b7ca-153">category</span></span>|[<span data-ttu-id="3b7ca-154">deviceAppManagementTaskCategory</span><span class="sxs-lookup"><span data-stu-id="3b7ca-154">deviceAppManagementTaskCategory</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskcategory.md)|<span data-ttu-id="3b7ca-155">Категория.</span><span class="sxs-lookup"><span data-stu-id="3b7ca-155">The category.</span></span> <span data-ttu-id="3b7ca-156">Наследуется [от deviceAppManagementTask.](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="3b7ca-156">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span></span> <span data-ttu-id="3b7ca-157">Возможные значения: `unknown`, `advancedThreatProtection`.</span><span class="sxs-lookup"><span data-stu-id="3b7ca-157">Possible values are: `unknown`, `advancedThreatProtection`.</span></span>|
|<span data-ttu-id="3b7ca-158">priority</span><span class="sxs-lookup"><span data-stu-id="3b7ca-158">priority</span></span>|[<span data-ttu-id="3b7ca-159">deviceAppManagementTaskPriority</span><span class="sxs-lookup"><span data-stu-id="3b7ca-159">deviceAppManagementTaskPriority</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskpriority.md)|<span data-ttu-id="3b7ca-160">Приоритет.</span><span class="sxs-lookup"><span data-stu-id="3b7ca-160">The priority.</span></span> <span data-ttu-id="3b7ca-161">Наследуется [от deviceAppManagementTask.](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="3b7ca-161">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span></span> <span data-ttu-id="3b7ca-162">Возможные значения: `none`, `high`, `low`.</span><span class="sxs-lookup"><span data-stu-id="3b7ca-162">Possible values are: `none`, `high`, `low`.</span></span>|
|<span data-ttu-id="3b7ca-163">creator</span><span class="sxs-lookup"><span data-stu-id="3b7ca-163">creator</span></span>|<span data-ttu-id="3b7ca-164">String</span><span class="sxs-lookup"><span data-stu-id="3b7ca-164">String</span></span>|<span data-ttu-id="3b7ca-165">Адрес электронной почты создателя.</span><span class="sxs-lookup"><span data-stu-id="3b7ca-165">The email address of the creator.</span></span> <span data-ttu-id="3b7ca-166">Наследуется [от deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="3b7ca-166">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="3b7ca-167">creatorNotes</span><span class="sxs-lookup"><span data-stu-id="3b7ca-167">creatorNotes</span></span>|<span data-ttu-id="3b7ca-168">String</span><span class="sxs-lookup"><span data-stu-id="3b7ca-168">String</span></span>|<span data-ttu-id="3b7ca-169">Примечания от создателя.</span><span class="sxs-lookup"><span data-stu-id="3b7ca-169">Notes from the creator.</span></span> <span data-ttu-id="3b7ca-170">Наследуется [от deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="3b7ca-170">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="3b7ca-171">assignedTo</span><span class="sxs-lookup"><span data-stu-id="3b7ca-171">assignedTo</span></span>|<span data-ttu-id="3b7ca-172">String</span><span class="sxs-lookup"><span data-stu-id="3b7ca-172">String</span></span>|<span data-ttu-id="3b7ca-173">Имя или адрес электронной почты администратора, для которого назначена эта задача.</span><span class="sxs-lookup"><span data-stu-id="3b7ca-173">The name or email of the admin this task is assigned to.</span></span> <span data-ttu-id="3b7ca-174">Наследуется [от deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="3b7ca-174">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="3b7ca-175">status</span><span class="sxs-lookup"><span data-stu-id="3b7ca-175">status</span></span>|[<span data-ttu-id="3b7ca-176">deviceAppManagementTaskStatus</span><span class="sxs-lookup"><span data-stu-id="3b7ca-176">deviceAppManagementTaskStatus</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskstatus.md)|<span data-ttu-id="3b7ca-177">Состояние.</span><span class="sxs-lookup"><span data-stu-id="3b7ca-177">The status.</span></span> <span data-ttu-id="3b7ca-178">Наследуется [от deviceAppManagementTask.](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="3b7ca-178">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span></span> <span data-ttu-id="3b7ca-179">Возможные значения: `unknown`, `pending`, `active`, `completed`, `rejected`.</span><span class="sxs-lookup"><span data-stu-id="3b7ca-179">Possible values are: `unknown`, `pending`, `active`, `completed`, `rejected`.</span></span>|
|<span data-ttu-id="3b7ca-180">unmanagedDevices</span><span class="sxs-lookup"><span data-stu-id="3b7ca-180">unmanagedDevices</span></span>|<span data-ttu-id="3b7ca-181">[коллекция unmanagedDevice](../resources/intune-partnerintegration-unmanageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="3b7ca-181">[unmanagedDevice](../resources/intune-partnerintegration-unmanageddevice.md) collection</span></span>|<span data-ttu-id="3b7ca-182">Неугодные устройства, обнаруженные в сети.</span><span class="sxs-lookup"><span data-stu-id="3b7ca-182">Unmanaged devices discovered in the network.</span></span>|



## <a name="response"></a><span data-ttu-id="3b7ca-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="3b7ca-183">Response</span></span>
<span data-ttu-id="3b7ca-184">В случае успеха этот метод возвращает код отклика и обновленный объект `200 OK` [unmanagedDeviceDiscoveryTask](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3b7ca-184">If successful, this method returns a `200 OK` response code and an updated [unmanagedDeviceDiscoveryTask](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b7ca-185">Пример</span><span class="sxs-lookup"><span data-stu-id="3b7ca-185">Example</span></span>

### <a name="request"></a><span data-ttu-id="3b7ca-186">Запрос</span><span class="sxs-lookup"><span data-stu-id="3b7ca-186">Request</span></span>
<span data-ttu-id="3b7ca-187">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3b7ca-187">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/deviceAppManagementTasks/{deviceAppManagementTaskId}
Content-type: application/json
Content-length: 961

{
  "@odata.type": "#microsoft.graph.unmanagedDeviceDiscoveryTask",
  "displayName": "Display Name value",
  "description": "Description value",
  "dueDateTime": "2017-01-01T00:02:18.1994089-08:00",
  "category": "advancedThreatProtection",
  "priority": "high",
  "creator": "Creator value",
  "creatorNotes": "Creator Notes value",
  "assignedTo": "Assigned To value",
  "status": "pending",
  "unmanagedDevices": [
    {
      "@odata.type": "microsoft.graph.unmanagedDevice",
      "os": "Os value",
      "osVersion": "Os Version value",
      "ipAddress": "Ip Address value",
      "deviceName": "Device Name value",
      "macAddress": "Mac Address value",
      "domain": "Domain value",
      "manufacturer": "Manufacturer value",
      "model": "Model value",
      "location": "Location value",
      "lastLoggedOnUser": "Last Logged On User value",
      "lastSeenDateTime": "2017-01-01T00:02:00.1006212-08:00"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="3b7ca-188">Отклик</span><span class="sxs-lookup"><span data-stu-id="3b7ca-188">Response</span></span>
<span data-ttu-id="3b7ca-p113">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3b7ca-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1069

{
  "@odata.type": "#microsoft.graph.unmanagedDeviceDiscoveryTask",
  "id": "6caa2ba0-2ba0-6caa-a02b-aa6ca02baa6c",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "dueDateTime": "2017-01-01T00:02:18.1994089-08:00",
  "category": "advancedThreatProtection",
  "priority": "high",
  "creator": "Creator value",
  "creatorNotes": "Creator Notes value",
  "assignedTo": "Assigned To value",
  "status": "pending",
  "unmanagedDevices": [
    {
      "@odata.type": "microsoft.graph.unmanagedDevice",
      "os": "Os value",
      "osVersion": "Os Version value",
      "ipAddress": "Ip Address value",
      "deviceName": "Device Name value",
      "macAddress": "Mac Address value",
      "domain": "Domain value",
      "manufacturer": "Manufacturer value",
      "model": "Model value",
      "location": "Location value",
      "lastLoggedOnUser": "Last Logged On User value",
      "lastSeenDateTime": "2017-01-01T00:02:00.1006212-08:00"
    }
  ]
}
```




