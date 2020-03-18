---
title: Обновление объекта mobileAppAssignment
description: Обновление свойств объекта mobileAppAssignment.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4b6c5ed81e61456514d6c3d80a2b172ea7cf5b83
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42761400"
---
# <a name="update-mobileappassignment"></a><span data-ttu-id="ddf08-103">Обновление объекта mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="ddf08-103">Update mobileAppAssignment</span></span>

> <span data-ttu-id="ddf08-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ddf08-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ddf08-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ddf08-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ddf08-106">Обновление свойств объекта [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ddf08-106">Update the properties of a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ddf08-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ddf08-107">Prerequisites</span></span>
<span data-ttu-id="ddf08-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ddf08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ddf08-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ddf08-110">Permission type</span></span>|<span data-ttu-id="ddf08-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ddf08-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ddf08-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ddf08-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ddf08-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddf08-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ddf08-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ddf08-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ddf08-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ddf08-115">Not supported.</span></span>|
|<span data-ttu-id="ddf08-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="ddf08-116">Application</span></span>|<span data-ttu-id="ddf08-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddf08-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ddf08-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ddf08-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="ddf08-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ddf08-119">Request headers</span></span>
|<span data-ttu-id="ddf08-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ddf08-120">Header</span></span>|<span data-ttu-id="ddf08-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ddf08-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ddf08-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ddf08-122">Authorization</span></span>|<span data-ttu-id="ddf08-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ddf08-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ddf08-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ddf08-124">Accept</span></span>|<span data-ttu-id="ddf08-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ddf08-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ddf08-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ddf08-126">Request body</span></span>
<span data-ttu-id="ddf08-127">В тексте запроса добавьте представление объекта [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ddf08-127">In the request body, supply a JSON representation for the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

<span data-ttu-id="ddf08-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ddf08-128">The following table shows the properties that are required when you create the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span></span>

|<span data-ttu-id="ddf08-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ddf08-129">Property</span></span>|<span data-ttu-id="ddf08-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ddf08-130">Type</span></span>|<span data-ttu-id="ddf08-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ddf08-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ddf08-132">id</span><span class="sxs-lookup"><span data-stu-id="ddf08-132">id</span></span>|<span data-ttu-id="ddf08-133">String</span><span class="sxs-lookup"><span data-stu-id="ddf08-133">String</span></span>|<span data-ttu-id="ddf08-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ddf08-134">Key of the entity.</span></span>|
|<span data-ttu-id="ddf08-135">intent</span><span class="sxs-lookup"><span data-stu-id="ddf08-135">intent</span></span>|[<span data-ttu-id="ddf08-136">installIntent</span><span class="sxs-lookup"><span data-stu-id="ddf08-136">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="ddf08-137">Цель установки, определенная администратором. Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="ddf08-137">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="ddf08-138">target</span><span class="sxs-lookup"><span data-stu-id="ddf08-138">target</span></span>|[<span data-ttu-id="ddf08-139">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="ddf08-139">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="ddf08-140">Целевое назначение группы, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="ddf08-140">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="ddf08-141">settings</span><span class="sxs-lookup"><span data-stu-id="ddf08-141">settings</span></span>|[<span data-ttu-id="ddf08-142">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="ddf08-142">mobileAppAssignmentSettings</span></span>](../resources/intune-shared-mobileappassignmentsettings.md)|<span data-ttu-id="ddf08-143">Параметры целевого назначения, определенные администратором.</span><span class="sxs-lookup"><span data-stu-id="ddf08-143">The settings for target assignment defined by the admin.</span></span>|
|<span data-ttu-id="ddf08-144">source</span><span class="sxs-lookup"><span data-stu-id="ddf08-144">source</span></span>|[<span data-ttu-id="ddf08-145">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="ddf08-145">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="ddf08-146">Тип ресурса, который является источником для назначения.</span><span class="sxs-lookup"><span data-stu-id="ddf08-146">The resource type which is the source for the assignment.</span></span> <span data-ttu-id="ddf08-147">Возможные значения: `direct`, `policySets`.</span><span class="sxs-lookup"><span data-stu-id="ddf08-147">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="ddf08-148">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="ddf08-148">sourceId</span></span>|<span data-ttu-id="ddf08-149">String</span><span class="sxs-lookup"><span data-stu-id="ddf08-149">String</span></span>|<span data-ttu-id="ddf08-150">Идентификатор источника назначения.</span><span class="sxs-lookup"><span data-stu-id="ddf08-150">The identifier of the source of the assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="ddf08-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="ddf08-151">Response</span></span>
<span data-ttu-id="ddf08-152">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ddf08-152">If successful, this method returns a `200 OK` response code and an updated [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ddf08-153">Пример</span><span class="sxs-lookup"><span data-stu-id="ddf08-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="ddf08-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="ddf08-154">Request</span></span>
<span data-ttu-id="ddf08-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ddf08-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
Content-type: application/json
Content-length: 334

{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "intent": "required",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```

### <a name="response"></a><span data-ttu-id="ddf08-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="ddf08-156">Response</span></span>
<span data-ttu-id="ddf08-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ddf08-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 383

{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "id": "591620b7-20b7-5916-b720-1659b7201659",
  "intent": "required",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```




