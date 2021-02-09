---
title: Обновление roleScopeTagAutoAssignment
description: Обновление свойств объекта roleScopeTagAutoAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 028fa830d45a961489c7dad9476c07839e21870e
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50153748"
---
# <a name="update-rolescopetagautoassignment"></a><span data-ttu-id="d6903-103">Обновление roleScopeTagAutoAssignment</span><span class="sxs-lookup"><span data-stu-id="d6903-103">Update roleScopeTagAutoAssignment</span></span>

<span data-ttu-id="d6903-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6903-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d6903-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6903-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6903-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d6903-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6903-107">Обновление свойств объекта [roleScopeTagAutoAssignment.](../resources/intune-rbac-rolescopetagautoassignment.md)</span><span class="sxs-lookup"><span data-stu-id="d6903-107">Update the properties of a [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d6903-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d6903-108">Prerequisites</span></span>
<span data-ttu-id="d6903-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6903-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6903-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d6903-111">Permission type</span></span>|<span data-ttu-id="d6903-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d6903-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6903-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d6903-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d6903-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6903-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="d6903-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d6903-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6903-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6903-116">Not supported.</span></span>|
|<span data-ttu-id="d6903-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d6903-117">Application</span></span>|<span data-ttu-id="d6903-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6903-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6903-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d6903-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}/assignments/{roleScopeTagAutoAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="d6903-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d6903-120">Request headers</span></span>
|<span data-ttu-id="d6903-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d6903-121">Header</span></span>|<span data-ttu-id="d6903-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d6903-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d6903-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d6903-123">Authorization</span></span>|<span data-ttu-id="d6903-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d6903-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d6903-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d6903-125">Accept</span></span>|<span data-ttu-id="d6903-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d6903-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6903-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d6903-127">Request body</span></span>
<span data-ttu-id="d6903-128">В теле запроса укажу представление объекта [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="d6903-128">In the request body, supply a JSON representation for the [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object.</span></span>

<span data-ttu-id="d6903-129">В следующей таблице показаны свойства, необходимые при создании [объекта roleScopeTagAutoAssignment.](../resources/intune-rbac-rolescopetagautoassignment.md)</span><span class="sxs-lookup"><span data-stu-id="d6903-129">The following table shows the properties that are required when you create the [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md).</span></span>

|<span data-ttu-id="d6903-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d6903-130">Property</span></span>|<span data-ttu-id="d6903-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d6903-131">Type</span></span>|<span data-ttu-id="d6903-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d6903-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6903-133">id</span><span class="sxs-lookup"><span data-stu-id="d6903-133">id</span></span>|<span data-ttu-id="d6903-134">String</span><span class="sxs-lookup"><span data-stu-id="d6903-134">String</span></span>|<span data-ttu-id="d6903-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d6903-135">Key of the entity.</span></span>|
|<span data-ttu-id="d6903-136">target</span><span class="sxs-lookup"><span data-stu-id="d6903-136">target</span></span>|[<span data-ttu-id="d6903-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d6903-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="d6903-138">Целевой объект автоматического назначения для определенного тега области роли.</span><span class="sxs-lookup"><span data-stu-id="d6903-138">The auto-assignment target for the specific Role Scope Tag.</span></span>|



## <a name="response"></a><span data-ttu-id="d6903-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6903-139">Response</span></span>
<span data-ttu-id="d6903-140">В случае успешного выполнения этот метод возвращает код отклика и обновленный объект `200 OK` [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d6903-140">If successful, this method returns a `200 OK` response code and an updated [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6903-141">Пример</span><span class="sxs-lookup"><span data-stu-id="d6903-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="d6903-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="d6903-142">Request</span></span>
<span data-ttu-id="d6903-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d6903-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d6903-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6903-144">Response</span></span>
<span data-ttu-id="d6903-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d6903-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




