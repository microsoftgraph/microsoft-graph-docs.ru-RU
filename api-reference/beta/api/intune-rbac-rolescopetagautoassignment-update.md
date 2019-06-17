---
title: Обновление Ролескопетагаутоассигнмент
description: Обновление свойств объекта Ролескопетагаутоассигнмент.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 69910087d50bfa2e9ae44b5632daeaf439ea62bd
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "35002478"
---
# <a name="update-rolescopetagautoassignment"></a><span data-ttu-id="f30d8-103">Обновление Ролескопетагаутоассигнмент</span><span class="sxs-lookup"><span data-stu-id="f30d8-103">Update roleScopeTagAutoAssignment</span></span>

> <span data-ttu-id="f30d8-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f30d8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f30d8-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f30d8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f30d8-106">Обновление свойств объекта [ролескопетагаутоассигнмент](../resources/intune-rbac-rolescopetagautoassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="f30d8-106">Update the properties of a [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f30d8-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f30d8-107">Prerequisites</span></span>
<span data-ttu-id="f30d8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f30d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f30d8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f30d8-110">Permission type</span></span>|<span data-ttu-id="f30d8-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f30d8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f30d8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f30d8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f30d8-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f30d8-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="f30d8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f30d8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f30d8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f30d8-115">Not supported.</span></span>|
|<span data-ttu-id="f30d8-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f30d8-116">Application</span></span>|<span data-ttu-id="f30d8-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f30d8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f30d8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f30d8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}/assignments/{roleScopeTagAutoAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="f30d8-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f30d8-119">Request headers</span></span>
|<span data-ttu-id="f30d8-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f30d8-120">Header</span></span>|<span data-ttu-id="f30d8-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f30d8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f30d8-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f30d8-122">Authorization</span></span>|<span data-ttu-id="f30d8-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f30d8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f30d8-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f30d8-124">Accept</span></span>|<span data-ttu-id="f30d8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f30d8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f30d8-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f30d8-126">Request body</span></span>
<span data-ttu-id="f30d8-127">В тексте запроса добавьте представление объекта [ролескопетагаутоассигнмент](../resources/intune-rbac-rolescopetagautoassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f30d8-127">In the request body, supply a JSON representation for the [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object.</span></span>

<span data-ttu-id="f30d8-128">В следующей таблице приведены свойства, необходимые при создании [ролескопетагаутоассигнмент](../resources/intune-rbac-rolescopetagautoassignment.md).</span><span class="sxs-lookup"><span data-stu-id="f30d8-128">The following table shows the properties that are required when you create the [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md).</span></span>

|<span data-ttu-id="f30d8-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="f30d8-129">Property</span></span>|<span data-ttu-id="f30d8-130">Тип</span><span class="sxs-lookup"><span data-stu-id="f30d8-130">Type</span></span>|<span data-ttu-id="f30d8-131">Описание</span><span class="sxs-lookup"><span data-stu-id="f30d8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f30d8-132">id</span><span class="sxs-lookup"><span data-stu-id="f30d8-132">id</span></span>|<span data-ttu-id="f30d8-133">String</span><span class="sxs-lookup"><span data-stu-id="f30d8-133">String</span></span>|<span data-ttu-id="f30d8-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f30d8-134">Key of the entity.</span></span>|
|<span data-ttu-id="f30d8-135">target</span><span class="sxs-lookup"><span data-stu-id="f30d8-135">target</span></span>|[<span data-ttu-id="f30d8-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="f30d8-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="f30d8-137">Целевой объект автоматического назначения для определенного тега области применения роли.</span><span class="sxs-lookup"><span data-stu-id="f30d8-137">The auto-assignment target for the specific Role Scope Tag.</span></span>|



## <a name="response"></a><span data-ttu-id="f30d8-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="f30d8-138">Response</span></span>
<span data-ttu-id="f30d8-139">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [ролескопетагаутоассигнмент](../resources/intune-rbac-rolescopetagautoassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f30d8-139">If successful, this method returns a `200 OK` response code and an updated [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f30d8-140">Пример</span><span class="sxs-lookup"><span data-stu-id="f30d8-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="f30d8-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="f30d8-141">Request</span></span>
<span data-ttu-id="f30d8-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f30d8-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}/assignments/{roleScopeTagAutoAssignmentId}
Content-type: application/json
Content-length: 166

{
  "@odata.type": "#microsoft.graph.roleScopeTagAutoAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="f30d8-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="f30d8-143">Response</span></span>
<span data-ttu-id="f30d8-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f30d8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 215

{
  "@odata.type": "#microsoft.graph.roleScopeTagAutoAssignment",
  "id": "256e6375-6375-256e-7563-6e2575636e25",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





