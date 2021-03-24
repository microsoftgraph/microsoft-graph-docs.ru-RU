---
title: Update roleScopeTagAutoAssignment
description: Обновление свойств объекта roleScopeTagAutoAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 919c9dee6eca38ee343809e13805ca8d3e623cac
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51134475"
---
# <a name="update-rolescopetagautoassignment"></a><span data-ttu-id="6fe45-103">Update roleScopeTagAutoAssignment</span><span class="sxs-lookup"><span data-stu-id="6fe45-103">Update roleScopeTagAutoAssignment</span></span>

<span data-ttu-id="6fe45-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6fe45-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6fe45-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6fe45-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6fe45-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6fe45-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6fe45-107">Обновление свойств объекта [roleScopeTagAutoAssignment.](../resources/intune-rbac-rolescopetagautoassignment.md)</span><span class="sxs-lookup"><span data-stu-id="6fe45-107">Update the properties of a [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6fe45-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6fe45-108">Prerequisites</span></span>
<span data-ttu-id="6fe45-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6fe45-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6fe45-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6fe45-111">Permission type</span></span>|<span data-ttu-id="6fe45-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6fe45-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6fe45-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6fe45-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6fe45-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6fe45-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="6fe45-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6fe45-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6fe45-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6fe45-116">Not supported.</span></span>|
|<span data-ttu-id="6fe45-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="6fe45-117">Application</span></span>|<span data-ttu-id="6fe45-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6fe45-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6fe45-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6fe45-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}/assignments/{roleScopeTagAutoAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="6fe45-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6fe45-120">Request headers</span></span>
|<span data-ttu-id="6fe45-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6fe45-121">Header</span></span>|<span data-ttu-id="6fe45-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6fe45-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6fe45-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6fe45-123">Authorization</span></span>|<span data-ttu-id="6fe45-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6fe45-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6fe45-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6fe45-125">Accept</span></span>|<span data-ttu-id="6fe45-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6fe45-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6fe45-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6fe45-127">Request body</span></span>
<span data-ttu-id="6fe45-128">В теле запроса поставляем представление JSON для объекта [roleScopeTagAutoAssignment.](../resources/intune-rbac-rolescopetagautoassignment.md)</span><span class="sxs-lookup"><span data-stu-id="6fe45-128">In the request body, supply a JSON representation for the [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object.</span></span>

<span data-ttu-id="6fe45-129">В следующей таблице показаны свойства, необходимые при создании [ролиScopeTagAutoAssignment.](../resources/intune-rbac-rolescopetagautoassignment.md)</span><span class="sxs-lookup"><span data-stu-id="6fe45-129">The following table shows the properties that are required when you create the [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md).</span></span>

|<span data-ttu-id="6fe45-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6fe45-130">Property</span></span>|<span data-ttu-id="6fe45-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6fe45-131">Type</span></span>|<span data-ttu-id="6fe45-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6fe45-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6fe45-133">id</span><span class="sxs-lookup"><span data-stu-id="6fe45-133">id</span></span>|<span data-ttu-id="6fe45-134">Строка</span><span class="sxs-lookup"><span data-stu-id="6fe45-134">String</span></span>|<span data-ttu-id="6fe45-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6fe45-135">Key of the entity.</span></span>|
|<span data-ttu-id="6fe45-136">target</span><span class="sxs-lookup"><span data-stu-id="6fe45-136">target</span></span>|[<span data-ttu-id="6fe45-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="6fe45-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="6fe45-138">Цель автоматического назначения для определенного тега области ролей.</span><span class="sxs-lookup"><span data-stu-id="6fe45-138">The auto-assignment target for the specific Role Scope Tag.</span></span>|



## <a name="response"></a><span data-ttu-id="6fe45-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="6fe45-139">Response</span></span>
<span data-ttu-id="6fe45-140">В случае успешного выполнения этот метод возвращает код отклика и обновленный объект `200 OK` [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="6fe45-140">If successful, this method returns a `200 OK` response code and an updated [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6fe45-141">Пример</span><span class="sxs-lookup"><span data-stu-id="6fe45-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="6fe45-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="6fe45-142">Request</span></span>
<span data-ttu-id="6fe45-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6fe45-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}/assignments/{roleScopeTagAutoAssignmentId}
Content-type: application/json
Content-length: 385

{
  "@odata.type": "#microsoft.graph.roleScopeTagAutoAssignment",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include",
    "collectionId": "Collection Id value"
  }
}
```

### <a name="response"></a><span data-ttu-id="6fe45-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="6fe45-144">Response</span></span>
<span data-ttu-id="6fe45-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6fe45-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 434

{
  "@odata.type": "#microsoft.graph.roleScopeTagAutoAssignment",
  "id": "256e6375-6375-256e-7563-6e2575636e25",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include",
    "collectionId": "Collection Id value"
  }
}
```




