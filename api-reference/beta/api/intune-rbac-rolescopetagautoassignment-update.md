---
title: Обновление Ролескопетагаутоассигнмент
description: Обновление свойств объекта Ролескопетагаутоассигнмент.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0860d28f77fcdadec1537e57ce1852ae20c8863a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49304471"
---
# <a name="update-rolescopetagautoassignment"></a><span data-ttu-id="8c230-103">Обновление Ролескопетагаутоассигнмент</span><span class="sxs-lookup"><span data-stu-id="8c230-103">Update roleScopeTagAutoAssignment</span></span>

<span data-ttu-id="8c230-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c230-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8c230-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c230-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8c230-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8c230-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c230-107">Обновление свойств объекта [ролескопетагаутоассигнмент](../resources/intune-rbac-rolescopetagautoassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="8c230-107">Update the properties of a [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8c230-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8c230-108">Prerequisites</span></span>
<span data-ttu-id="8c230-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c230-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c230-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8c230-111">Permission type</span></span>|<span data-ttu-id="8c230-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8c230-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c230-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8c230-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8c230-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c230-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="8c230-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8c230-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c230-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c230-116">Not supported.</span></span>|
|<span data-ttu-id="8c230-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8c230-117">Application</span></span>|<span data-ttu-id="8c230-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c230-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c230-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8c230-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}/assignments/{roleScopeTagAutoAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="8c230-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8c230-120">Request headers</span></span>
|<span data-ttu-id="8c230-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8c230-121">Header</span></span>|<span data-ttu-id="8c230-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8c230-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8c230-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8c230-123">Authorization</span></span>|<span data-ttu-id="8c230-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8c230-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8c230-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8c230-125">Accept</span></span>|<span data-ttu-id="8c230-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8c230-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c230-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8c230-127">Request body</span></span>
<span data-ttu-id="8c230-128">В тексте запроса добавьте представление объекта [ролескопетагаутоассигнмент](../resources/intune-rbac-rolescopetagautoassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8c230-128">In the request body, supply a JSON representation for the [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object.</span></span>

<span data-ttu-id="8c230-129">В следующей таблице приведены свойства, необходимые при создании [ролескопетагаутоассигнмент](../resources/intune-rbac-rolescopetagautoassignment.md).</span><span class="sxs-lookup"><span data-stu-id="8c230-129">The following table shows the properties that are required when you create the [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md).</span></span>

|<span data-ttu-id="8c230-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8c230-130">Property</span></span>|<span data-ttu-id="8c230-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8c230-131">Type</span></span>|<span data-ttu-id="8c230-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8c230-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c230-133">id</span><span class="sxs-lookup"><span data-stu-id="8c230-133">id</span></span>|<span data-ttu-id="8c230-134">String</span><span class="sxs-lookup"><span data-stu-id="8c230-134">String</span></span>|<span data-ttu-id="8c230-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8c230-135">Key of the entity.</span></span>|
|<span data-ttu-id="8c230-136">target</span><span class="sxs-lookup"><span data-stu-id="8c230-136">target</span></span>|[<span data-ttu-id="8c230-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="8c230-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="8c230-138">Целевой объект автоматического назначения для определенного тега области применения роли.</span><span class="sxs-lookup"><span data-stu-id="8c230-138">The auto-assignment target for the specific Role Scope Tag.</span></span>|



## <a name="response"></a><span data-ttu-id="8c230-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c230-139">Response</span></span>
<span data-ttu-id="8c230-140">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [ролескопетагаутоассигнмент](../resources/intune-rbac-rolescopetagautoassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8c230-140">If successful, this method returns a `200 OK` response code and an updated [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c230-141">Пример</span><span class="sxs-lookup"><span data-stu-id="8c230-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="8c230-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="8c230-142">Request</span></span>
<span data-ttu-id="8c230-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8c230-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}/assignments/{roleScopeTagAutoAssignmentId}
Content-type: application/json
Content-length: 321

{
  "@odata.type": "#microsoft.graph.roleScopeTagAutoAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```

### <a name="response"></a><span data-ttu-id="8c230-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c230-144">Response</span></span>
<span data-ttu-id="8c230-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8c230-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 370

{
  "@odata.type": "#microsoft.graph.roleScopeTagAutoAssignment",
  "id": "256e6375-6375-256e-7563-6e2575636e25",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```




