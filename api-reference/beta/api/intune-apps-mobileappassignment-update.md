---
title: Обновление объекта mobileAppAssignment
description: Обновление свойств объекта mobileAppAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d94b0447b2dcf4de967f2eeb6e40534ac1a579bc
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51139883"
---
# <a name="update-mobileappassignment"></a><span data-ttu-id="47d4f-103">Обновление объекта mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="47d4f-103">Update mobileAppAssignment</span></span>

<span data-ttu-id="47d4f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47d4f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="47d4f-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47d4f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="47d4f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="47d4f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47d4f-107">Обновление свойств объекта [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="47d4f-107">Update the properties of a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="47d4f-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="47d4f-108">Prerequisites</span></span>
<span data-ttu-id="47d4f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47d4f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47d4f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="47d4f-111">Permission type</span></span>|<span data-ttu-id="47d4f-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="47d4f-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47d4f-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="47d4f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="47d4f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47d4f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="47d4f-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="47d4f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47d4f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47d4f-116">Not supported.</span></span>|
|<span data-ttu-id="47d4f-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="47d4f-117">Application</span></span>|<span data-ttu-id="47d4f-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47d4f-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="47d4f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="47d4f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="47d4f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="47d4f-120">Request headers</span></span>
|<span data-ttu-id="47d4f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="47d4f-121">Header</span></span>|<span data-ttu-id="47d4f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="47d4f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="47d4f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="47d4f-123">Authorization</span></span>|<span data-ttu-id="47d4f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="47d4f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="47d4f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="47d4f-125">Accept</span></span>|<span data-ttu-id="47d4f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="47d4f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="47d4f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="47d4f-127">Request body</span></span>
<span data-ttu-id="47d4f-128">В тексте запроса добавьте представление объекта [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="47d4f-128">In the request body, supply a JSON representation for the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

<span data-ttu-id="47d4f-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="47d4f-129">The following table shows the properties that are required when you create the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span></span>

|<span data-ttu-id="47d4f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="47d4f-130">Property</span></span>|<span data-ttu-id="47d4f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="47d4f-131">Type</span></span>|<span data-ttu-id="47d4f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="47d4f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47d4f-133">id</span><span class="sxs-lookup"><span data-stu-id="47d4f-133">id</span></span>|<span data-ttu-id="47d4f-134">Строка</span><span class="sxs-lookup"><span data-stu-id="47d4f-134">String</span></span>|<span data-ttu-id="47d4f-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="47d4f-135">Key of the entity.</span></span>|
|<span data-ttu-id="47d4f-136">intent</span><span class="sxs-lookup"><span data-stu-id="47d4f-136">intent</span></span>|[<span data-ttu-id="47d4f-137">installIntent</span><span class="sxs-lookup"><span data-stu-id="47d4f-137">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="47d4f-138">Цель установки, определенная администратором. Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="47d4f-138">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="47d4f-139">target</span><span class="sxs-lookup"><span data-stu-id="47d4f-139">target</span></span>|[<span data-ttu-id="47d4f-140">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="47d4f-140">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="47d4f-141">Целевое назначение группы, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="47d4f-141">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="47d4f-142">settings</span><span class="sxs-lookup"><span data-stu-id="47d4f-142">settings</span></span>|[<span data-ttu-id="47d4f-143">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="47d4f-143">mobileAppAssignmentSettings</span></span>](../resources/intune-shared-mobileappassignmentsettings.md)|<span data-ttu-id="47d4f-144">Параметры целевого назначения, определенные администратором.</span><span class="sxs-lookup"><span data-stu-id="47d4f-144">The settings for target assignment defined by the admin.</span></span>|
|<span data-ttu-id="47d4f-145">source</span><span class="sxs-lookup"><span data-stu-id="47d4f-145">source</span></span>|[<span data-ttu-id="47d4f-146">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="47d4f-146">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="47d4f-147">Тип ресурса, который является источником назначения.</span><span class="sxs-lookup"><span data-stu-id="47d4f-147">The resource type which is the source for the assignment.</span></span> <span data-ttu-id="47d4f-148">Возможные значения: `direct`, `policySets`.</span><span class="sxs-lookup"><span data-stu-id="47d4f-148">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="47d4f-149">sourceId</span><span class="sxs-lookup"><span data-stu-id="47d4f-149">sourceId</span></span>|<span data-ttu-id="47d4f-150">Строка</span><span class="sxs-lookup"><span data-stu-id="47d4f-150">String</span></span>|<span data-ttu-id="47d4f-151">Идентификатор источника назначения.</span><span class="sxs-lookup"><span data-stu-id="47d4f-151">The identifier of the source of the assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="47d4f-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="47d4f-152">Response</span></span>
<span data-ttu-id="47d4f-153">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="47d4f-153">If successful, this method returns a `200 OK` response code and an updated [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47d4f-154">Пример</span><span class="sxs-lookup"><span data-stu-id="47d4f-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="47d4f-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="47d4f-155">Request</span></span>
<span data-ttu-id="47d4f-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="47d4f-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
Content-type: application/json
Content-length: 617

{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "intent": "required",
  "target": {
    "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  },
  "settings": {
    "@odata.type": "microsoft.graph.iosLobAppAssignmentSettings",
    "vpnConfigurationId": "Vpn Configuration Id value",
    "uninstallOnDeviceRemoval": true,
    "isRemovable": true
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```

### <a name="response"></a><span data-ttu-id="47d4f-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="47d4f-157">Response</span></span>
<span data-ttu-id="47d4f-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="47d4f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 666

{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "id": "591620b7-20b7-5916-b720-1659b7201659",
  "intent": "required",
  "target": {
    "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  },
  "settings": {
    "@odata.type": "microsoft.graph.iosLobAppAssignmentSettings",
    "vpnConfigurationId": "Vpn Configuration Id value",
    "uninstallOnDeviceRemoval": true,
    "isRemovable": true
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```




