---
title: Обновление deviceManagementResourceAccessProfileAssignment
description: Обновление свойств объекта deviceManagementResourceAccessProfileAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1cc09d3d66ba27ae440688a7a18bbfdc3bbd1246
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161994"
---
# <a name="update-devicemanagementresourceaccessprofileassignment"></a><span data-ttu-id="9a339-103">Обновление deviceManagementResourceAccessProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="9a339-103">Update deviceManagementResourceAccessProfileAssignment</span></span>

<span data-ttu-id="9a339-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a339-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9a339-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a339-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9a339-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9a339-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a339-107">Обновление свойств объекта [deviceManagementResourceAccessProfileAssignment.](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md)</span><span class="sxs-lookup"><span data-stu-id="9a339-107">Update the properties of a [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9a339-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9a339-108">Prerequisites</span></span>
<span data-ttu-id="9a339-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a339-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a339-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9a339-111">Permission type</span></span>|<span data-ttu-id="9a339-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9a339-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9a339-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9a339-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9a339-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a339-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9a339-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9a339-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9a339-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a339-116">Not supported.</span></span>|
|<span data-ttu-id="9a339-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9a339-117">Application</span></span>|<span data-ttu-id="9a339-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a339-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9a339-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9a339-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/resourceAccessProfiles/{deviceManagementResourceAccessProfileBaseId}/assignments/{deviceManagementResourceAccessProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="9a339-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9a339-120">Request headers</span></span>
|<span data-ttu-id="9a339-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9a339-121">Header</span></span>|<span data-ttu-id="9a339-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9a339-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9a339-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9a339-123">Authorization</span></span>|<span data-ttu-id="9a339-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9a339-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9a339-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9a339-125">Accept</span></span>|<span data-ttu-id="9a339-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9a339-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a339-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9a339-127">Request body</span></span>
<span data-ttu-id="9a339-128">В теле запроса укажу представление объекта [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="9a339-128">In the request body, supply a JSON representation for the [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) object.</span></span>

<span data-ttu-id="9a339-129">В следующей таблице показаны свойства, необходимые при создании [объекта deviceManagementResourceAccessProfileAssignment.](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md)</span><span class="sxs-lookup"><span data-stu-id="9a339-129">The following table shows the properties that are required when you create the [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md).</span></span>

|<span data-ttu-id="9a339-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9a339-130">Property</span></span>|<span data-ttu-id="9a339-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9a339-131">Type</span></span>|<span data-ttu-id="9a339-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9a339-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a339-133">id</span><span class="sxs-lookup"><span data-stu-id="9a339-133">id</span></span>|<span data-ttu-id="9a339-134">String</span><span class="sxs-lookup"><span data-stu-id="9a339-134">String</span></span>|<span data-ttu-id="9a339-135">Уникальный идентификатор для назначений</span><span class="sxs-lookup"><span data-stu-id="9a339-135">Unique identifier for the Assignments</span></span>|
|<span data-ttu-id="9a339-136">intent</span><span class="sxs-lookup"><span data-stu-id="9a339-136">intent</span></span>|[<span data-ttu-id="9a339-137">deviceManagementResourceAccessProfileIntent</span><span class="sxs-lookup"><span data-stu-id="9a339-137">deviceManagementResourceAccessProfileIntent</span></span>](../resources/intune-rapolicy-devicemanagementresourceaccessprofileintent.md)|<span data-ttu-id="9a339-138">Назначение профиля доступа к ресурсам.</span><span class="sxs-lookup"><span data-stu-id="9a339-138">The assignment intent for the resource access profile.</span></span> <span data-ttu-id="9a339-139">Возможные значения: `apply`, `remove`.</span><span class="sxs-lookup"><span data-stu-id="9a339-139">Possible values are: `apply`, `remove`.</span></span>|
|<span data-ttu-id="9a339-140">target</span><span class="sxs-lookup"><span data-stu-id="9a339-140">target</span></span>|[<span data-ttu-id="9a339-141">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="9a339-141">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="9a339-142">Целевой объект назначения для профиля доступа к ресурсам.</span><span class="sxs-lookup"><span data-stu-id="9a339-142">The assignment target for the resource access profile.</span></span>|
|<span data-ttu-id="9a339-143">sourceId</span><span class="sxs-lookup"><span data-stu-id="9a339-143">sourceId</span></span>|<span data-ttu-id="9a339-144">String</span><span class="sxs-lookup"><span data-stu-id="9a339-144">String</span></span>|<span data-ttu-id="9a339-145">Идентификатор источника назначения.</span><span class="sxs-lookup"><span data-stu-id="9a339-145">The identifier of the source of the assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="9a339-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a339-146">Response</span></span>
<span data-ttu-id="9a339-147">В случае успешного выполнения этот метод возвращает код отклика и обновленный объект `200 OK` [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9a339-147">If successful, this method returns a `200 OK` response code and an updated [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a339-148">Пример</span><span class="sxs-lookup"><span data-stu-id="9a339-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="9a339-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="9a339-149">Request</span></span>
<span data-ttu-id="9a339-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9a339-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/resourceAccessProfiles/{deviceManagementResourceAccessProfileBaseId}/assignments/{deviceManagementResourceAccessProfileAssignmentId}
Content-type: application/json
Content-length: 463

{
  "@odata.type": "#microsoft.graph.deviceManagementResourceAccessProfileAssignment",
  "intent": "remove",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include",
    "collectionId": "Collection Id value"
  },
  "sourceId": "Source Id value"
}
```

### <a name="response"></a><span data-ttu-id="9a339-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a339-151">Response</span></span>
<span data-ttu-id="9a339-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9a339-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 512

{
  "@odata.type": "#microsoft.graph.deviceManagementResourceAccessProfileAssignment",
  "id": "4ebb8d4e-8d4e-4ebb-4e8d-bb4e4e8dbb4e",
  "intent": "remove",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include",
    "collectionId": "Collection Id value"
  },
  "sourceId": "Source Id value"
}
```




