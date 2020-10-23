---
title: Создание объекта mobileAppAssignment
description: Создание объекта mobileAppAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d72b4e21881b0813f0ac4808b8052df6072df9c5
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48699053"
---
# <a name="create-mobileappassignment"></a><span data-ttu-id="d1c09-103">Создание объекта mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="d1c09-103">Create mobileAppAssignment</span></span>

<span data-ttu-id="d1c09-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1c09-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d1c09-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1c09-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d1c09-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d1c09-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1c09-107">Создание объекта [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d1c09-107">Create a new [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d1c09-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d1c09-108">Prerequisites</span></span>
<span data-ttu-id="d1c09-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1c09-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1c09-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d1c09-111">Permission type</span></span>|<span data-ttu-id="d1c09-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d1c09-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d1c09-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d1c09-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d1c09-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1c09-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d1c09-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d1c09-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d1c09-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1c09-116">Not supported.</span></span>|
|<span data-ttu-id="d1c09-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d1c09-117">Application</span></span>|<span data-ttu-id="d1c09-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1c09-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d1c09-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d1c09-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="d1c09-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d1c09-120">Request headers</span></span>
|<span data-ttu-id="d1c09-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d1c09-121">Header</span></span>|<span data-ttu-id="d1c09-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d1c09-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d1c09-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d1c09-123">Authorization</span></span>|<span data-ttu-id="d1c09-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d1c09-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d1c09-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d1c09-125">Accept</span></span>|<span data-ttu-id="d1c09-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d1c09-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1c09-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d1c09-127">Request body</span></span>
<span data-ttu-id="d1c09-128">В тексте запроса добавьте представление объекта mobileAppAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d1c09-128">In the request body, supply a JSON representation for the mobileAppAssignment object.</span></span>

<span data-ttu-id="d1c09-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта mobileAppAssignment.</span><span class="sxs-lookup"><span data-stu-id="d1c09-129">The following table shows the properties that are required when you create the mobileAppAssignment.</span></span>

|<span data-ttu-id="d1c09-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d1c09-130">Property</span></span>|<span data-ttu-id="d1c09-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d1c09-131">Type</span></span>|<span data-ttu-id="d1c09-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d1c09-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1c09-133">id</span><span class="sxs-lookup"><span data-stu-id="d1c09-133">id</span></span>|<span data-ttu-id="d1c09-134">Строка</span><span class="sxs-lookup"><span data-stu-id="d1c09-134">String</span></span>|<span data-ttu-id="d1c09-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d1c09-135">Key of the entity.</span></span>|
|<span data-ttu-id="d1c09-136">intent</span><span class="sxs-lookup"><span data-stu-id="d1c09-136">intent</span></span>|[<span data-ttu-id="d1c09-137">installIntent</span><span class="sxs-lookup"><span data-stu-id="d1c09-137">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="d1c09-138">Цель установки, определенная администратором. Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="d1c09-138">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="d1c09-139">target</span><span class="sxs-lookup"><span data-stu-id="d1c09-139">target</span></span>|[<span data-ttu-id="d1c09-140">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d1c09-140">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="d1c09-141">Целевое назначение группы, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="d1c09-141">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="d1c09-142">settings</span><span class="sxs-lookup"><span data-stu-id="d1c09-142">settings</span></span>|[<span data-ttu-id="d1c09-143">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="d1c09-143">mobileAppAssignmentSettings</span></span>](../resources/intune-shared-mobileappassignmentsettings.md)|<span data-ttu-id="d1c09-144">Параметры целевого назначения, определенные администратором.</span><span class="sxs-lookup"><span data-stu-id="d1c09-144">The settings for target assignment defined by the admin.</span></span>|
|<span data-ttu-id="d1c09-145">source</span><span class="sxs-lookup"><span data-stu-id="d1c09-145">source</span></span>|[<span data-ttu-id="d1c09-146">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="d1c09-146">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="d1c09-147">Тип ресурса, который является источником для назначения.</span><span class="sxs-lookup"><span data-stu-id="d1c09-147">The resource type which is the source for the assignment.</span></span> <span data-ttu-id="d1c09-148">Возможные значения: `direct`, `policySets`.</span><span class="sxs-lookup"><span data-stu-id="d1c09-148">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="d1c09-149">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="d1c09-149">sourceId</span></span>|<span data-ttu-id="d1c09-150">Строка</span><span class="sxs-lookup"><span data-stu-id="d1c09-150">String</span></span>|<span data-ttu-id="d1c09-151">Идентификатор источника назначения.</span><span class="sxs-lookup"><span data-stu-id="d1c09-151">The identifier of the source of the assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="d1c09-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1c09-152">Response</span></span>
<span data-ttu-id="d1c09-153">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d1c09-153">If successful, this method returns a `201 Created` response code and a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1c09-154">Пример</span><span class="sxs-lookup"><span data-stu-id="d1c09-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="d1c09-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="d1c09-155">Request</span></span>
<span data-ttu-id="d1c09-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d1c09-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d1c09-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1c09-157">Response</span></span>
<span data-ttu-id="d1c09-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d1c09-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





