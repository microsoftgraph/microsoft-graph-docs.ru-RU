---
title: Создание объекта mobileAppAssignment
description: Создание объекта mobileAppAssignment.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f5a3894b183d8edae03091f65c535d504d9f9932
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42761428"
---
# <a name="create-mobileappassignment"></a><span data-ttu-id="3e1ec-103">Создание объекта mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="3e1ec-103">Create mobileAppAssignment</span></span>

> <span data-ttu-id="3e1ec-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e1ec-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3e1ec-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3e1ec-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e1ec-106">Создание объекта [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="3e1ec-106">Create a new [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3e1ec-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="3e1ec-107">Prerequisites</span></span>
<span data-ttu-id="3e1ec-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e1ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e1ec-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3e1ec-110">Permission type</span></span>|<span data-ttu-id="3e1ec-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3e1ec-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3e1ec-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3e1ec-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3e1ec-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e1ec-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3e1ec-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3e1ec-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3e1ec-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e1ec-115">Not supported.</span></span>|
|<span data-ttu-id="3e1ec-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="3e1ec-116">Application</span></span>|<span data-ttu-id="3e1ec-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e1ec-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3e1ec-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3e1ec-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="3e1ec-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3e1ec-119">Request headers</span></span>
|<span data-ttu-id="3e1ec-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3e1ec-120">Header</span></span>|<span data-ttu-id="3e1ec-121">Значение</span><span class="sxs-lookup"><span data-stu-id="3e1ec-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3e1ec-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e1ec-122">Authorization</span></span>|<span data-ttu-id="3e1ec-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3e1ec-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3e1ec-124">Accept</span><span class="sxs-lookup"><span data-stu-id="3e1ec-124">Accept</span></span>|<span data-ttu-id="3e1ec-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3e1ec-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e1ec-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3e1ec-126">Request body</span></span>
<span data-ttu-id="3e1ec-127">В тексте запроса добавьте представление объекта mobileAppAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3e1ec-127">In the request body, supply a JSON representation for the mobileAppAssignment object.</span></span>

<span data-ttu-id="3e1ec-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта mobileAppAssignment.</span><span class="sxs-lookup"><span data-stu-id="3e1ec-128">The following table shows the properties that are required when you create the mobileAppAssignment.</span></span>

|<span data-ttu-id="3e1ec-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="3e1ec-129">Property</span></span>|<span data-ttu-id="3e1ec-130">Тип</span><span class="sxs-lookup"><span data-stu-id="3e1ec-130">Type</span></span>|<span data-ttu-id="3e1ec-131">Описание</span><span class="sxs-lookup"><span data-stu-id="3e1ec-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e1ec-132">id</span><span class="sxs-lookup"><span data-stu-id="3e1ec-132">id</span></span>|<span data-ttu-id="3e1ec-133">String</span><span class="sxs-lookup"><span data-stu-id="3e1ec-133">String</span></span>|<span data-ttu-id="3e1ec-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3e1ec-134">Key of the entity.</span></span>|
|<span data-ttu-id="3e1ec-135">intent</span><span class="sxs-lookup"><span data-stu-id="3e1ec-135">intent</span></span>|[<span data-ttu-id="3e1ec-136">installIntent</span><span class="sxs-lookup"><span data-stu-id="3e1ec-136">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="3e1ec-137">Цель установки, определенная администратором. Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="3e1ec-137">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="3e1ec-138">target</span><span class="sxs-lookup"><span data-stu-id="3e1ec-138">target</span></span>|[<span data-ttu-id="3e1ec-139">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="3e1ec-139">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="3e1ec-140">Целевое назначение группы, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="3e1ec-140">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="3e1ec-141">settings</span><span class="sxs-lookup"><span data-stu-id="3e1ec-141">settings</span></span>|[<span data-ttu-id="3e1ec-142">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="3e1ec-142">mobileAppAssignmentSettings</span></span>](../resources/intune-shared-mobileappassignmentsettings.md)|<span data-ttu-id="3e1ec-143">Параметры целевого назначения, определенные администратором.</span><span class="sxs-lookup"><span data-stu-id="3e1ec-143">The settings for target assignment defined by the admin.</span></span>|
|<span data-ttu-id="3e1ec-144">source</span><span class="sxs-lookup"><span data-stu-id="3e1ec-144">source</span></span>|[<span data-ttu-id="3e1ec-145">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="3e1ec-145">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="3e1ec-146">Тип ресурса, который является источником для назначения.</span><span class="sxs-lookup"><span data-stu-id="3e1ec-146">The resource type which is the source for the assignment.</span></span> <span data-ttu-id="3e1ec-147">Возможные значения: `direct`, `policySets`.</span><span class="sxs-lookup"><span data-stu-id="3e1ec-147">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="3e1ec-148">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="3e1ec-148">sourceId</span></span>|<span data-ttu-id="3e1ec-149">String</span><span class="sxs-lookup"><span data-stu-id="3e1ec-149">String</span></span>|<span data-ttu-id="3e1ec-150">Идентификатор источника назначения.</span><span class="sxs-lookup"><span data-stu-id="3e1ec-150">The identifier of the source of the assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="3e1ec-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e1ec-151">Response</span></span>
<span data-ttu-id="3e1ec-152">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3e1ec-152">If successful, this method returns a `201 Created` response code and a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e1ec-153">Пример</span><span class="sxs-lookup"><span data-stu-id="3e1ec-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="3e1ec-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="3e1ec-154">Request</span></span>
<span data-ttu-id="3e1ec-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3e1ec-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/assignments
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

### <a name="response"></a><span data-ttu-id="3e1ec-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e1ec-156">Response</span></span>
<span data-ttu-id="3e1ec-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3e1ec-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




