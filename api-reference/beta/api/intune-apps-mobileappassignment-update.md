---
title: Обновление объекта mobileAppAssignment
description: Обновление свойств объекта mobileAppAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1b43aff448c7db5a6665b0fdafd4921e8fb774c7
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793320"
---
# <a name="update-mobileappassignment"></a><span data-ttu-id="55491-103">Обновление объекта mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="55491-103">Update mobileAppAssignment</span></span>

<span data-ttu-id="55491-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55491-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="55491-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55491-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="55491-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="55491-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55491-107">Обновление свойств объекта [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="55491-107">Update the properties of a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="55491-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="55491-108">Prerequisites</span></span>
<span data-ttu-id="55491-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55491-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55491-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="55491-111">Permission type</span></span>|<span data-ttu-id="55491-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="55491-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="55491-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="55491-113">Delegated (work or school account)</span></span>|<span data-ttu-id="55491-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55491-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="55491-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="55491-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="55491-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55491-116">Not supported.</span></span>|
|<span data-ttu-id="55491-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="55491-117">Application</span></span>|<span data-ttu-id="55491-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55491-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="55491-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="55491-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="55491-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="55491-120">Request headers</span></span>
|<span data-ttu-id="55491-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="55491-121">Header</span></span>|<span data-ttu-id="55491-122">Значение</span><span class="sxs-lookup"><span data-stu-id="55491-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="55491-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="55491-123">Authorization</span></span>|<span data-ttu-id="55491-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="55491-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="55491-125">Accept</span><span class="sxs-lookup"><span data-stu-id="55491-125">Accept</span></span>|<span data-ttu-id="55491-126">application/json</span><span class="sxs-lookup"><span data-stu-id="55491-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="55491-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="55491-127">Request body</span></span>
<span data-ttu-id="55491-128">В тексте запроса добавьте представление объекта [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="55491-128">In the request body, supply a JSON representation for the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

<span data-ttu-id="55491-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="55491-129">The following table shows the properties that are required when you create the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span></span>

|<span data-ttu-id="55491-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="55491-130">Property</span></span>|<span data-ttu-id="55491-131">Тип</span><span class="sxs-lookup"><span data-stu-id="55491-131">Type</span></span>|<span data-ttu-id="55491-132">Описание</span><span class="sxs-lookup"><span data-stu-id="55491-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55491-133">id</span><span class="sxs-lookup"><span data-stu-id="55491-133">id</span></span>|<span data-ttu-id="55491-134">String</span><span class="sxs-lookup"><span data-stu-id="55491-134">String</span></span>|<span data-ttu-id="55491-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="55491-135">Key of the entity.</span></span>|
|<span data-ttu-id="55491-136">intent</span><span class="sxs-lookup"><span data-stu-id="55491-136">intent</span></span>|[<span data-ttu-id="55491-137">installIntent</span><span class="sxs-lookup"><span data-stu-id="55491-137">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="55491-138">Цель установки, определенная администратором. Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="55491-138">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="55491-139">target</span><span class="sxs-lookup"><span data-stu-id="55491-139">target</span></span>|[<span data-ttu-id="55491-140">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="55491-140">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="55491-141">Целевое назначение группы, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="55491-141">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="55491-142">settings</span><span class="sxs-lookup"><span data-stu-id="55491-142">settings</span></span>|[<span data-ttu-id="55491-143">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="55491-143">mobileAppAssignmentSettings</span></span>](../resources/intune-shared-mobileappassignmentsettings.md)|<span data-ttu-id="55491-144">Параметры целевого назначения, определенные администратором.</span><span class="sxs-lookup"><span data-stu-id="55491-144">The settings for target assignment defined by the admin.</span></span>|
|<span data-ttu-id="55491-145">source</span><span class="sxs-lookup"><span data-stu-id="55491-145">source</span></span>|[<span data-ttu-id="55491-146">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="55491-146">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="55491-147">Тип ресурса, который является источником для назначения.</span><span class="sxs-lookup"><span data-stu-id="55491-147">The resource type which is the source for the assignment.</span></span> <span data-ttu-id="55491-148">Возможные значения: `direct`, `policySets`.</span><span class="sxs-lookup"><span data-stu-id="55491-148">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="55491-149">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="55491-149">sourceId</span></span>|<span data-ttu-id="55491-150">String</span><span class="sxs-lookup"><span data-stu-id="55491-150">String</span></span>|<span data-ttu-id="55491-151">Идентификатор источника назначения.</span><span class="sxs-lookup"><span data-stu-id="55491-151">The identifier of the source of the assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="55491-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="55491-152">Response</span></span>
<span data-ttu-id="55491-153">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="55491-153">If successful, this method returns a `200 OK` response code and an updated [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55491-154">Пример</span><span class="sxs-lookup"><span data-stu-id="55491-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="55491-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="55491-155">Request</span></span>
<span data-ttu-id="55491-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="55491-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
Content-type: application/json
Content-length: 591

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
    "uninstallOnDeviceRemoval": true
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```

### <a name="response"></a><span data-ttu-id="55491-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="55491-157">Response</span></span>
<span data-ttu-id="55491-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="55491-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 640

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
    "uninstallOnDeviceRemoval": true
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```



