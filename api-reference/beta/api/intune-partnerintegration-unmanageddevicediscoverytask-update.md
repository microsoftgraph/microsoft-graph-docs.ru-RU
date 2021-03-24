---
title: Обновление unmanagedDeviceDiscoveryTask
description: Обновление свойств объекта unmanagedDeviceDiscoveryTask.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 87722cb838dcc46d7275c8de3530a7d1792b6e3d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51141780"
---
# <a name="update-unmanageddevicediscoverytask"></a><span data-ttu-id="505c5-103">Обновление unmanagedDeviceDiscoveryTask</span><span class="sxs-lookup"><span data-stu-id="505c5-103">Update unmanagedDeviceDiscoveryTask</span></span>

<span data-ttu-id="505c5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="505c5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="505c5-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="505c5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="505c5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="505c5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="505c5-107">Обновление свойств объекта [unmanagedDeviceDiscoveryTask.](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md)</span><span class="sxs-lookup"><span data-stu-id="505c5-107">Update the properties of a [unmanagedDeviceDiscoveryTask](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="505c5-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="505c5-108">Prerequisites</span></span>
<span data-ttu-id="505c5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="505c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="505c5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="505c5-111">Permission type</span></span>|<span data-ttu-id="505c5-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="505c5-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="505c5-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="505c5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="505c5-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="505c5-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="505c5-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="505c5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="505c5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="505c5-116">Not supported.</span></span>|
|<span data-ttu-id="505c5-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="505c5-117">Application</span></span>|<span data-ttu-id="505c5-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="505c5-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="505c5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="505c5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/deviceAppManagementTasks/{deviceAppManagementTaskId}
```

## <a name="request-headers"></a><span data-ttu-id="505c5-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="505c5-120">Request headers</span></span>
|<span data-ttu-id="505c5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="505c5-121">Header</span></span>|<span data-ttu-id="505c5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="505c5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="505c5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="505c5-123">Authorization</span></span>|<span data-ttu-id="505c5-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="505c5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="505c5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="505c5-125">Accept</span></span>|<span data-ttu-id="505c5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="505c5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="505c5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="505c5-127">Request body</span></span>
<span data-ttu-id="505c5-128">В теле запроса поставляем представление JSON для объекта [unmanagedDeviceDiscoveryTask.](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md)</span><span class="sxs-lookup"><span data-stu-id="505c5-128">In the request body, supply a JSON representation for the [unmanagedDeviceDiscoveryTask](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md) object.</span></span>

<span data-ttu-id="505c5-129">В следующей таблице показаны свойства, необходимые при создании [unmanagedDeviceDiscoveryTask.](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md)</span><span class="sxs-lookup"><span data-stu-id="505c5-129">The following table shows the properties that are required when you create the [unmanagedDeviceDiscoveryTask](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md).</span></span>

|<span data-ttu-id="505c5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="505c5-130">Property</span></span>|<span data-ttu-id="505c5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="505c5-131">Type</span></span>|<span data-ttu-id="505c5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="505c5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="505c5-133">id</span><span class="sxs-lookup"><span data-stu-id="505c5-133">id</span></span>|<span data-ttu-id="505c5-134">Строка</span><span class="sxs-lookup"><span data-stu-id="505c5-134">String</span></span>|<span data-ttu-id="505c5-135">Ключ сущности.</span><span class="sxs-lookup"><span data-stu-id="505c5-135">The entity key.</span></span> <span data-ttu-id="505c5-136">Унаследованный от [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="505c5-136">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="505c5-137">displayName</span><span class="sxs-lookup"><span data-stu-id="505c5-137">displayName</span></span>|<span data-ttu-id="505c5-138">Строка</span><span class="sxs-lookup"><span data-stu-id="505c5-138">String</span></span>|<span data-ttu-id="505c5-139">Имя.</span><span class="sxs-lookup"><span data-stu-id="505c5-139">The name.</span></span> <span data-ttu-id="505c5-140">Унаследованный от [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="505c5-140">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="505c5-141">description</span><span class="sxs-lookup"><span data-stu-id="505c5-141">description</span></span>|<span data-ttu-id="505c5-142">Строка</span><span class="sxs-lookup"><span data-stu-id="505c5-142">String</span></span>|<span data-ttu-id="505c5-143">Описание.</span><span class="sxs-lookup"><span data-stu-id="505c5-143">The description.</span></span> <span data-ttu-id="505c5-144">Унаследованный от [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="505c5-144">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="505c5-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="505c5-145">createdDateTime</span></span>|<span data-ttu-id="505c5-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="505c5-146">DateTimeOffset</span></span>|<span data-ttu-id="505c5-147">Дата создания.</span><span class="sxs-lookup"><span data-stu-id="505c5-147">The created date.</span></span> <span data-ttu-id="505c5-148">Унаследованный от [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="505c5-148">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="505c5-149">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="505c5-149">dueDateTime</span></span>|<span data-ttu-id="505c5-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="505c5-150">DateTimeOffset</span></span>|<span data-ttu-id="505c5-151">Срок действия.</span><span class="sxs-lookup"><span data-stu-id="505c5-151">The due date.</span></span> <span data-ttu-id="505c5-152">Унаследованный от [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="505c5-152">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="505c5-153">category</span><span class="sxs-lookup"><span data-stu-id="505c5-153">category</span></span>|[<span data-ttu-id="505c5-154">deviceAppManagementTaskCategory</span><span class="sxs-lookup"><span data-stu-id="505c5-154">deviceAppManagementTaskCategory</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskcategory.md)|<span data-ttu-id="505c5-155">Категория.</span><span class="sxs-lookup"><span data-stu-id="505c5-155">The category.</span></span> <span data-ttu-id="505c5-156">Унаследовано от [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span><span class="sxs-lookup"><span data-stu-id="505c5-156">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span></span> <span data-ttu-id="505c5-157">Возможные значения: `unknown`, `advancedThreatProtection`.</span><span class="sxs-lookup"><span data-stu-id="505c5-157">Possible values are: `unknown`, `advancedThreatProtection`.</span></span>|
|<span data-ttu-id="505c5-158">priority</span><span class="sxs-lookup"><span data-stu-id="505c5-158">priority</span></span>|[<span data-ttu-id="505c5-159">deviceAppManagementTaskPriority</span><span class="sxs-lookup"><span data-stu-id="505c5-159">deviceAppManagementTaskPriority</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskpriority.md)|<span data-ttu-id="505c5-160">Приоритет.</span><span class="sxs-lookup"><span data-stu-id="505c5-160">The priority.</span></span> <span data-ttu-id="505c5-161">Унаследовано от [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span><span class="sxs-lookup"><span data-stu-id="505c5-161">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span></span> <span data-ttu-id="505c5-162">Возможные значения: `none`, `high`, `low`.</span><span class="sxs-lookup"><span data-stu-id="505c5-162">Possible values are: `none`, `high`, `low`.</span></span>|
|<span data-ttu-id="505c5-163">creator</span><span class="sxs-lookup"><span data-stu-id="505c5-163">creator</span></span>|<span data-ttu-id="505c5-164">Строка</span><span class="sxs-lookup"><span data-stu-id="505c5-164">String</span></span>|<span data-ttu-id="505c5-165">Адрес электронной почты создателя.</span><span class="sxs-lookup"><span data-stu-id="505c5-165">The email address of the creator.</span></span> <span data-ttu-id="505c5-166">Унаследованный от [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="505c5-166">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="505c5-167">creatorNotes</span><span class="sxs-lookup"><span data-stu-id="505c5-167">creatorNotes</span></span>|<span data-ttu-id="505c5-168">Строка</span><span class="sxs-lookup"><span data-stu-id="505c5-168">String</span></span>|<span data-ttu-id="505c5-169">Заметки от создателя.</span><span class="sxs-lookup"><span data-stu-id="505c5-169">Notes from the creator.</span></span> <span data-ttu-id="505c5-170">Унаследованный от [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="505c5-170">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="505c5-171">assignedTo</span><span class="sxs-lookup"><span data-stu-id="505c5-171">assignedTo</span></span>|<span data-ttu-id="505c5-172">String</span><span class="sxs-lookup"><span data-stu-id="505c5-172">String</span></span>|<span data-ttu-id="505c5-173">Имя или электронная почта администратора этой задачи назначены.</span><span class="sxs-lookup"><span data-stu-id="505c5-173">The name or email of the admin this task is assigned to.</span></span> <span data-ttu-id="505c5-174">Унаследованный от [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="505c5-174">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="505c5-175">status</span><span class="sxs-lookup"><span data-stu-id="505c5-175">status</span></span>|[<span data-ttu-id="505c5-176">deviceAppManagementTaskStatus</span><span class="sxs-lookup"><span data-stu-id="505c5-176">deviceAppManagementTaskStatus</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskstatus.md)|<span data-ttu-id="505c5-177">Состояние.</span><span class="sxs-lookup"><span data-stu-id="505c5-177">The status.</span></span> <span data-ttu-id="505c5-178">Унаследовано от [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span><span class="sxs-lookup"><span data-stu-id="505c5-178">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span></span> <span data-ttu-id="505c5-179">Возможные значения: `unknown`, `pending`, `active`, `completed`, `rejected`.</span><span class="sxs-lookup"><span data-stu-id="505c5-179">Possible values are: `unknown`, `pending`, `active`, `completed`, `rejected`.</span></span>|
|<span data-ttu-id="505c5-180">unmanagedDevices</span><span class="sxs-lookup"><span data-stu-id="505c5-180">unmanagedDevices</span></span>|<span data-ttu-id="505c5-181">[коллекция unmanagedDevice](../resources/intune-partnerintegration-unmanageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="505c5-181">[unmanagedDevice](../resources/intune-partnerintegration-unmanageddevice.md) collection</span></span>|<span data-ttu-id="505c5-182">Неугодные устройства, обнаруженные в сети.</span><span class="sxs-lookup"><span data-stu-id="505c5-182">Unmanaged devices discovered in the network.</span></span>|



## <a name="response"></a><span data-ttu-id="505c5-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="505c5-183">Response</span></span>
<span data-ttu-id="505c5-184">В случае успешной работы этот метод возвращает код отклика и обновленный объект `200 OK` [unmanagedDeviceDiscoveryTask](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="505c5-184">If successful, this method returns a `200 OK` response code and an updated [unmanagedDeviceDiscoveryTask](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="505c5-185">Пример</span><span class="sxs-lookup"><span data-stu-id="505c5-185">Example</span></span>

### <a name="request"></a><span data-ttu-id="505c5-186">Запрос</span><span class="sxs-lookup"><span data-stu-id="505c5-186">Request</span></span>
<span data-ttu-id="505c5-187">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="505c5-187">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="505c5-188">Отклик</span><span class="sxs-lookup"><span data-stu-id="505c5-188">Response</span></span>
<span data-ttu-id="505c5-p113">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="505c5-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




