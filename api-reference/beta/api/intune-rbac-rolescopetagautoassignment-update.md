---
title: Обновление Ролескопетагаутоассигнмент
description: Обновление свойств объекта Ролескопетагаутоассигнмент.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3d347acd7b7b6f4f22e9cc2ae55a05c26c8cc7af
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48698402"
---
# <a name="update-rolescopetagautoassignment"></a><span data-ttu-id="6845b-103">Обновление Ролескопетагаутоассигнмент</span><span class="sxs-lookup"><span data-stu-id="6845b-103">Update roleScopeTagAutoAssignment</span></span>

<span data-ttu-id="6845b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6845b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6845b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6845b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6845b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6845b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6845b-107">Обновление свойств объекта [ролескопетагаутоассигнмент](../resources/intune-rbac-rolescopetagautoassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="6845b-107">Update the properties of a [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6845b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6845b-108">Prerequisites</span></span>
<span data-ttu-id="6845b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6845b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6845b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6845b-111">Permission type</span></span>|<span data-ttu-id="6845b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6845b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6845b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6845b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6845b-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6845b-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="6845b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6845b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6845b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6845b-116">Not supported.</span></span>|
|<span data-ttu-id="6845b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6845b-117">Application</span></span>|<span data-ttu-id="6845b-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6845b-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6845b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6845b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}/assignments/{roleScopeTagAutoAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="6845b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6845b-120">Request headers</span></span>
|<span data-ttu-id="6845b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6845b-121">Header</span></span>|<span data-ttu-id="6845b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6845b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6845b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6845b-123">Authorization</span></span>|<span data-ttu-id="6845b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6845b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6845b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6845b-125">Accept</span></span>|<span data-ttu-id="6845b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6845b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6845b-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6845b-127">Request body</span></span>
<span data-ttu-id="6845b-128">В тексте запроса добавьте представление объекта [ролескопетагаутоассигнмент](../resources/intune-rbac-rolescopetagautoassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6845b-128">In the request body, supply a JSON representation for the [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object.</span></span>

<span data-ttu-id="6845b-129">В следующей таблице приведены свойства, необходимые при создании [ролескопетагаутоассигнмент](../resources/intune-rbac-rolescopetagautoassignment.md).</span><span class="sxs-lookup"><span data-stu-id="6845b-129">The following table shows the properties that are required when you create the [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md).</span></span>

|<span data-ttu-id="6845b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6845b-130">Property</span></span>|<span data-ttu-id="6845b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6845b-131">Type</span></span>|<span data-ttu-id="6845b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6845b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6845b-133">id</span><span class="sxs-lookup"><span data-stu-id="6845b-133">id</span></span>|<span data-ttu-id="6845b-134">Строка</span><span class="sxs-lookup"><span data-stu-id="6845b-134">String</span></span>|<span data-ttu-id="6845b-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6845b-135">Key of the entity.</span></span>|
|<span data-ttu-id="6845b-136">target</span><span class="sxs-lookup"><span data-stu-id="6845b-136">target</span></span>|[<span data-ttu-id="6845b-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="6845b-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="6845b-138">Целевой объект автоматического назначения для определенного тега области применения роли.</span><span class="sxs-lookup"><span data-stu-id="6845b-138">The auto-assignment target for the specific Role Scope Tag.</span></span>|



## <a name="response"></a><span data-ttu-id="6845b-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="6845b-139">Response</span></span>
<span data-ttu-id="6845b-140">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [ролескопетагаутоассигнмент](../resources/intune-rbac-rolescopetagautoassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6845b-140">If successful, this method returns a `200 OK` response code and an updated [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6845b-141">Пример</span><span class="sxs-lookup"><span data-stu-id="6845b-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="6845b-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="6845b-142">Request</span></span>
<span data-ttu-id="6845b-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6845b-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6845b-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="6845b-144">Response</span></span>
<span data-ttu-id="6845b-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6845b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





