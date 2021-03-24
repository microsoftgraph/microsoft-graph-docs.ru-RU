---
title: Создание объекта managedDeviceMobileAppConfigurationAssignment
description: Создание объекта managedDeviceMobileAppConfigurationAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6f255230467b3efb6d31a0b1739b699d5e9e7b7b
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51140212"
---
# <a name="create-manageddevicemobileappconfigurationassignment"></a><span data-ttu-id="66a27-103">Создание объекта managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="66a27-103">Create managedDeviceMobileAppConfigurationAssignment</span></span>

<span data-ttu-id="66a27-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66a27-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="66a27-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66a27-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="66a27-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="66a27-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66a27-107">Создание объекта [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="66a27-107">Create a new [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="66a27-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="66a27-108">Prerequisites</span></span>
<span data-ttu-id="66a27-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66a27-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66a27-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="66a27-111">Permission type</span></span>|<span data-ttu-id="66a27-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="66a27-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="66a27-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="66a27-113">Delegated (work or school account)</span></span>|<span data-ttu-id="66a27-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66a27-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="66a27-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="66a27-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="66a27-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66a27-116">Not supported.</span></span>|
|<span data-ttu-id="66a27-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="66a27-117">Application</span></span>|<span data-ttu-id="66a27-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66a27-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="66a27-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="66a27-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="66a27-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="66a27-120">Request headers</span></span>
|<span data-ttu-id="66a27-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="66a27-121">Header</span></span>|<span data-ttu-id="66a27-122">Значение</span><span class="sxs-lookup"><span data-stu-id="66a27-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="66a27-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="66a27-123">Authorization</span></span>|<span data-ttu-id="66a27-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="66a27-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="66a27-125">Accept</span><span class="sxs-lookup"><span data-stu-id="66a27-125">Accept</span></span>|<span data-ttu-id="66a27-126">application/json</span><span class="sxs-lookup"><span data-stu-id="66a27-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="66a27-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="66a27-127">Request body</span></span>
<span data-ttu-id="66a27-128">В тексте запроса добавьте представление объекта managedDeviceMobileAppConfigurationAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="66a27-128">In the request body, supply a JSON representation for the managedDeviceMobileAppConfigurationAssignment object.</span></span>

<span data-ttu-id="66a27-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта managedDeviceMobileAppConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="66a27-129">The following table shows the properties that are required when you create the managedDeviceMobileAppConfigurationAssignment.</span></span>

|<span data-ttu-id="66a27-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="66a27-130">Property</span></span>|<span data-ttu-id="66a27-131">Тип</span><span class="sxs-lookup"><span data-stu-id="66a27-131">Type</span></span>|<span data-ttu-id="66a27-132">Описание</span><span class="sxs-lookup"><span data-stu-id="66a27-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66a27-133">id</span><span class="sxs-lookup"><span data-stu-id="66a27-133">id</span></span>|<span data-ttu-id="66a27-134">Строка</span><span class="sxs-lookup"><span data-stu-id="66a27-134">String</span></span>|<span data-ttu-id="66a27-135">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="66a27-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="66a27-136">target</span><span class="sxs-lookup"><span data-stu-id="66a27-136">target</span></span>|[<span data-ttu-id="66a27-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="66a27-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="66a27-138">Объект, для которого назначается политика соблюдения условий.</span><span class="sxs-lookup"><span data-stu-id="66a27-138">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="66a27-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="66a27-139">Response</span></span>
<span data-ttu-id="66a27-140">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="66a27-140">If successful, this method returns a `201 Created` response code and a [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66a27-141">Пример</span><span class="sxs-lookup"><span data-stu-id="66a27-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="66a27-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="66a27-142">Request</span></span>
<span data-ttu-id="66a27-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="66a27-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
Content-type: application/json
Content-length: 346

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```

### <a name="response"></a><span data-ttu-id="66a27-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="66a27-144">Response</span></span>
<span data-ttu-id="66a27-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="66a27-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 395

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
  "id": "4df81c9c-1c9c-4df8-9c1c-f84d9c1cf84d",
  "target": {
    "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```




