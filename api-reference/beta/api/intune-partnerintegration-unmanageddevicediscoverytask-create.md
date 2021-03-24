---
title: Создание unmanagedDeviceDiscoveryTask
description: Создайте новый объект unmanagedDeviceDiscoveryTask.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 032b1e19e72dae2a30f125ab5c030098a23d8ad6
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51134804"
---
# <a name="create-unmanageddevicediscoverytask"></a><span data-ttu-id="b6164-103">Создание unmanagedDeviceDiscoveryTask</span><span class="sxs-lookup"><span data-stu-id="b6164-103">Create unmanagedDeviceDiscoveryTask</span></span>

<span data-ttu-id="b6164-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6164-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b6164-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6164-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b6164-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b6164-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6164-107">Создайте новый [объект unmanagedDeviceDiscoveryTask.](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md)</span><span class="sxs-lookup"><span data-stu-id="b6164-107">Create a new [unmanagedDeviceDiscoveryTask](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b6164-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b6164-108">Prerequisites</span></span>
<span data-ttu-id="b6164-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6164-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6164-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b6164-111">Permission type</span></span>|<span data-ttu-id="b6164-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b6164-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6164-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b6164-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b6164-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6164-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b6164-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b6164-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6164-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6164-116">Not supported.</span></span>|
|<span data-ttu-id="b6164-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="b6164-117">Application</span></span>|<span data-ttu-id="b6164-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6164-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6164-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b6164-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/deviceAppManagementTasks
```

## <a name="request-headers"></a><span data-ttu-id="b6164-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b6164-120">Request headers</span></span>
|<span data-ttu-id="b6164-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b6164-121">Header</span></span>|<span data-ttu-id="b6164-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b6164-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6164-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b6164-123">Authorization</span></span>|<span data-ttu-id="b6164-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b6164-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6164-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b6164-125">Accept</span></span>|<span data-ttu-id="b6164-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b6164-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6164-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b6164-127">Request body</span></span>
<span data-ttu-id="b6164-128">В теле запроса поставляем представление JSON для объекта unmanagedDeviceDiscoveryTask.</span><span class="sxs-lookup"><span data-stu-id="b6164-128">In the request body, supply a JSON representation for the unmanagedDeviceDiscoveryTask object.</span></span>

<span data-ttu-id="b6164-129">В следующей таблице показаны свойства, необходимые при создании unmanagedDeviceDiscoveryTask.</span><span class="sxs-lookup"><span data-stu-id="b6164-129">The following table shows the properties that are required when you create the unmanagedDeviceDiscoveryTask.</span></span>

|<span data-ttu-id="b6164-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b6164-130">Property</span></span>|<span data-ttu-id="b6164-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b6164-131">Type</span></span>|<span data-ttu-id="b6164-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b6164-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6164-133">id</span><span class="sxs-lookup"><span data-stu-id="b6164-133">id</span></span>|<span data-ttu-id="b6164-134">Строка</span><span class="sxs-lookup"><span data-stu-id="b6164-134">String</span></span>|<span data-ttu-id="b6164-135">Ключ сущности.</span><span class="sxs-lookup"><span data-stu-id="b6164-135">The entity key.</span></span> <span data-ttu-id="b6164-136">Унаследованный от [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="b6164-136">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="b6164-137">displayName</span><span class="sxs-lookup"><span data-stu-id="b6164-137">displayName</span></span>|<span data-ttu-id="b6164-138">Строка</span><span class="sxs-lookup"><span data-stu-id="b6164-138">String</span></span>|<span data-ttu-id="b6164-139">Имя.</span><span class="sxs-lookup"><span data-stu-id="b6164-139">The name.</span></span> <span data-ttu-id="b6164-140">Унаследованный от [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="b6164-140">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="b6164-141">description</span><span class="sxs-lookup"><span data-stu-id="b6164-141">description</span></span>|<span data-ttu-id="b6164-142">Строка</span><span class="sxs-lookup"><span data-stu-id="b6164-142">String</span></span>|<span data-ttu-id="b6164-143">Описание.</span><span class="sxs-lookup"><span data-stu-id="b6164-143">The description.</span></span> <span data-ttu-id="b6164-144">Унаследованный от [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="b6164-144">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="b6164-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b6164-145">createdDateTime</span></span>|<span data-ttu-id="b6164-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6164-146">DateTimeOffset</span></span>|<span data-ttu-id="b6164-147">Дата создания.</span><span class="sxs-lookup"><span data-stu-id="b6164-147">The created date.</span></span> <span data-ttu-id="b6164-148">Унаследованный от [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="b6164-148">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="b6164-149">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="b6164-149">dueDateTime</span></span>|<span data-ttu-id="b6164-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6164-150">DateTimeOffset</span></span>|<span data-ttu-id="b6164-151">Срок действия.</span><span class="sxs-lookup"><span data-stu-id="b6164-151">The due date.</span></span> <span data-ttu-id="b6164-152">Унаследованный от [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="b6164-152">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="b6164-153">category</span><span class="sxs-lookup"><span data-stu-id="b6164-153">category</span></span>|[<span data-ttu-id="b6164-154">deviceAppManagementTaskCategory</span><span class="sxs-lookup"><span data-stu-id="b6164-154">deviceAppManagementTaskCategory</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskcategory.md)|<span data-ttu-id="b6164-155">Категория.</span><span class="sxs-lookup"><span data-stu-id="b6164-155">The category.</span></span> <span data-ttu-id="b6164-156">Унаследовано от [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span><span class="sxs-lookup"><span data-stu-id="b6164-156">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span></span> <span data-ttu-id="b6164-157">Возможные значения: `unknown`, `advancedThreatProtection`.</span><span class="sxs-lookup"><span data-stu-id="b6164-157">Possible values are: `unknown`, `advancedThreatProtection`.</span></span>|
|<span data-ttu-id="b6164-158">priority</span><span class="sxs-lookup"><span data-stu-id="b6164-158">priority</span></span>|[<span data-ttu-id="b6164-159">deviceAppManagementTaskPriority</span><span class="sxs-lookup"><span data-stu-id="b6164-159">deviceAppManagementTaskPriority</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskpriority.md)|<span data-ttu-id="b6164-160">Приоритет.</span><span class="sxs-lookup"><span data-stu-id="b6164-160">The priority.</span></span> <span data-ttu-id="b6164-161">Унаследовано от [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span><span class="sxs-lookup"><span data-stu-id="b6164-161">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span></span> <span data-ttu-id="b6164-162">Возможные значения: `none`, `high`, `low`.</span><span class="sxs-lookup"><span data-stu-id="b6164-162">Possible values are: `none`, `high`, `low`.</span></span>|
|<span data-ttu-id="b6164-163">creator</span><span class="sxs-lookup"><span data-stu-id="b6164-163">creator</span></span>|<span data-ttu-id="b6164-164">Строка</span><span class="sxs-lookup"><span data-stu-id="b6164-164">String</span></span>|<span data-ttu-id="b6164-165">Адрес электронной почты создателя.</span><span class="sxs-lookup"><span data-stu-id="b6164-165">The email address of the creator.</span></span> <span data-ttu-id="b6164-166">Унаследованный от [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="b6164-166">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="b6164-167">creatorNotes</span><span class="sxs-lookup"><span data-stu-id="b6164-167">creatorNotes</span></span>|<span data-ttu-id="b6164-168">Строка</span><span class="sxs-lookup"><span data-stu-id="b6164-168">String</span></span>|<span data-ttu-id="b6164-169">Заметки от создателя.</span><span class="sxs-lookup"><span data-stu-id="b6164-169">Notes from the creator.</span></span> <span data-ttu-id="b6164-170">Унаследованный от [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="b6164-170">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="b6164-171">assignedTo</span><span class="sxs-lookup"><span data-stu-id="b6164-171">assignedTo</span></span>|<span data-ttu-id="b6164-172">String</span><span class="sxs-lookup"><span data-stu-id="b6164-172">String</span></span>|<span data-ttu-id="b6164-173">Имя или электронная почта администратора этой задачи назначены.</span><span class="sxs-lookup"><span data-stu-id="b6164-173">The name or email of the admin this task is assigned to.</span></span> <span data-ttu-id="b6164-174">Унаследованный от [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="b6164-174">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="b6164-175">status</span><span class="sxs-lookup"><span data-stu-id="b6164-175">status</span></span>|[<span data-ttu-id="b6164-176">deviceAppManagementTaskStatus</span><span class="sxs-lookup"><span data-stu-id="b6164-176">deviceAppManagementTaskStatus</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskstatus.md)|<span data-ttu-id="b6164-177">Состояние.</span><span class="sxs-lookup"><span data-stu-id="b6164-177">The status.</span></span> <span data-ttu-id="b6164-178">Унаследовано от [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span><span class="sxs-lookup"><span data-stu-id="b6164-178">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span></span> <span data-ttu-id="b6164-179">Возможные значения: `unknown`, `pending`, `active`, `completed`, `rejected`.</span><span class="sxs-lookup"><span data-stu-id="b6164-179">Possible values are: `unknown`, `pending`, `active`, `completed`, `rejected`.</span></span>|
|<span data-ttu-id="b6164-180">unmanagedDevices</span><span class="sxs-lookup"><span data-stu-id="b6164-180">unmanagedDevices</span></span>|<span data-ttu-id="b6164-181">[коллекция unmanagedDevice](../resources/intune-partnerintegration-unmanageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="b6164-181">[unmanagedDevice](../resources/intune-partnerintegration-unmanageddevice.md) collection</span></span>|<span data-ttu-id="b6164-182">Неугодные устройства, обнаруженные в сети.</span><span class="sxs-lookup"><span data-stu-id="b6164-182">Unmanaged devices discovered in the network.</span></span>|



## <a name="response"></a><span data-ttu-id="b6164-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="b6164-183">Response</span></span>
<span data-ttu-id="b6164-184">В случае успешной работы этот метод возвращает код ответа и объект `201 Created` [unmanagedDeviceDiscoveryTask](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b6164-184">If successful, this method returns a `201 Created` response code and a [unmanagedDeviceDiscoveryTask](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6164-185">Пример</span><span class="sxs-lookup"><span data-stu-id="b6164-185">Example</span></span>

### <a name="request"></a><span data-ttu-id="b6164-186">Запрос</span><span class="sxs-lookup"><span data-stu-id="b6164-186">Request</span></span>
<span data-ttu-id="b6164-187">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b6164-187">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/deviceAppManagementTasks
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

### <a name="response"></a><span data-ttu-id="b6164-188">Отклик</span><span class="sxs-lookup"><span data-stu-id="b6164-188">Response</span></span>
<span data-ttu-id="b6164-p113">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b6164-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




