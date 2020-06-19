---
title: Создание объекта mobileAppAssignment
description: Создание объекта mobileAppAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9e0a1d5bb75374307362b5291233afb5b554b6fe
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793341"
---
# <a name="create-mobileappassignment"></a><span data-ttu-id="ac06e-103">Создание объекта mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="ac06e-103">Create mobileAppAssignment</span></span>

<span data-ttu-id="ac06e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac06e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ac06e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ac06e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ac06e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ac06e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ac06e-107">Создание объекта [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ac06e-107">Create a new [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ac06e-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ac06e-108">Prerequisites</span></span>
<span data-ttu-id="ac06e-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="ac06e-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="ac06e-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac06e-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ac06e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ac06e-111">Permission type</span></span>|<span data-ttu-id="ac06e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ac06e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ac06e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ac06e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ac06e-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac06e-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ac06e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ac06e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ac06e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ac06e-116">Not supported.</span></span>|
|<span data-ttu-id="ac06e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ac06e-117">Application</span></span>|<span data-ttu-id="ac06e-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac06e-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ac06e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ac06e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="ac06e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ac06e-120">Request headers</span></span>
|<span data-ttu-id="ac06e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ac06e-121">Header</span></span>|<span data-ttu-id="ac06e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ac06e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ac06e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ac06e-123">Authorization</span></span>|<span data-ttu-id="ac06e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ac06e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ac06e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ac06e-125">Accept</span></span>|<span data-ttu-id="ac06e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ac06e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ac06e-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ac06e-127">Request body</span></span>
<span data-ttu-id="ac06e-128">В тексте запроса добавьте представление объекта mobileAppAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ac06e-128">In the request body, supply a JSON representation for the mobileAppAssignment object.</span></span>

<span data-ttu-id="ac06e-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта mobileAppAssignment.</span><span class="sxs-lookup"><span data-stu-id="ac06e-129">The following table shows the properties that are required when you create the mobileAppAssignment.</span></span>

|<span data-ttu-id="ac06e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ac06e-130">Property</span></span>|<span data-ttu-id="ac06e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ac06e-131">Type</span></span>|<span data-ttu-id="ac06e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ac06e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac06e-133">id</span><span class="sxs-lookup"><span data-stu-id="ac06e-133">id</span></span>|<span data-ttu-id="ac06e-134">String</span><span class="sxs-lookup"><span data-stu-id="ac06e-134">String</span></span>|<span data-ttu-id="ac06e-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ac06e-135">Key of the entity.</span></span>|
|<span data-ttu-id="ac06e-136">intent</span><span class="sxs-lookup"><span data-stu-id="ac06e-136">intent</span></span>|[<span data-ttu-id="ac06e-137">installIntent</span><span class="sxs-lookup"><span data-stu-id="ac06e-137">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="ac06e-138">Цель установки, определенная администратором. Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="ac06e-138">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="ac06e-139">target</span><span class="sxs-lookup"><span data-stu-id="ac06e-139">target</span></span>|[<span data-ttu-id="ac06e-140">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="ac06e-140">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="ac06e-141">Целевое назначение группы, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="ac06e-141">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="ac06e-142">settings</span><span class="sxs-lookup"><span data-stu-id="ac06e-142">settings</span></span>|[<span data-ttu-id="ac06e-143">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="ac06e-143">mobileAppAssignmentSettings</span></span>](../resources/intune-shared-mobileappassignmentsettings.md)|<span data-ttu-id="ac06e-144">Параметры целевого назначения, определенные администратором.</span><span class="sxs-lookup"><span data-stu-id="ac06e-144">The settings for target assignment defined by the admin.</span></span>|
|<span data-ttu-id="ac06e-145">source</span><span class="sxs-lookup"><span data-stu-id="ac06e-145">source</span></span>|[<span data-ttu-id="ac06e-146">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="ac06e-146">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="ac06e-147">Тип ресурса, который является источником для назначения.</span><span class="sxs-lookup"><span data-stu-id="ac06e-147">The resource type which is the source for the assignment.</span></span> <span data-ttu-id="ac06e-148">Возможные значения: `direct`, `policySets`.</span><span class="sxs-lookup"><span data-stu-id="ac06e-148">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="ac06e-149">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="ac06e-149">sourceId</span></span>|<span data-ttu-id="ac06e-150">String</span><span class="sxs-lookup"><span data-stu-id="ac06e-150">String</span></span>|<span data-ttu-id="ac06e-151">Идентификатор источника назначения.</span><span class="sxs-lookup"><span data-stu-id="ac06e-151">The identifier of the source of the assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="ac06e-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac06e-152">Response</span></span>
<span data-ttu-id="ac06e-153">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ac06e-153">If successful, this method returns a `201 Created` response code and a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac06e-154">Пример</span><span class="sxs-lookup"><span data-stu-id="ac06e-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="ac06e-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="ac06e-155">Request</span></span>
<span data-ttu-id="ac06e-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ac06e-156">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/assignments
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

### <a name="response"></a><span data-ttu-id="ac06e-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac06e-157">Response</span></span>
<span data-ttu-id="ac06e-158">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="ac06e-158">Here is an example of the response.</span></span> <span data-ttu-id="ac06e-159">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="ac06e-159">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="ac06e-160">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="ac06e-160">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



