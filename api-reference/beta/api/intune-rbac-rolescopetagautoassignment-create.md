---
title: Создание Ролескопетагаутоассигнмент
description: Создание нового объекта Ролескопетагаутоассигнмент.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b18b5e5af1f3a65485c633145cd5288c4bf7c070
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43437580"
---
# <a name="create-rolescopetagautoassignment"></a><span data-ttu-id="c2d65-103">Создание Ролескопетагаутоассигнмент</span><span class="sxs-lookup"><span data-stu-id="c2d65-103">Create roleScopeTagAutoAssignment</span></span>

<span data-ttu-id="c2d65-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2d65-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c2d65-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2d65-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c2d65-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c2d65-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2d65-107">Создание нового объекта [ролескопетагаутоассигнмент](../resources/intune-rbac-rolescopetagautoassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="c2d65-107">Create a new [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c2d65-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c2d65-108">Prerequisites</span></span>
<span data-ttu-id="c2d65-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2d65-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2d65-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c2d65-111">Permission type</span></span>|<span data-ttu-id="c2d65-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c2d65-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c2d65-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c2d65-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c2d65-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2d65-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="c2d65-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c2d65-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c2d65-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2d65-116">Not supported.</span></span>|
|<span data-ttu-id="c2d65-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c2d65-117">Application</span></span>|<span data-ttu-id="c2d65-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2d65-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c2d65-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c2d65-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="c2d65-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c2d65-120">Request headers</span></span>
|<span data-ttu-id="c2d65-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c2d65-121">Header</span></span>|<span data-ttu-id="c2d65-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c2d65-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c2d65-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c2d65-123">Authorization</span></span>|<span data-ttu-id="c2d65-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c2d65-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c2d65-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c2d65-125">Accept</span></span>|<span data-ttu-id="c2d65-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c2d65-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2d65-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c2d65-127">Request body</span></span>
<span data-ttu-id="c2d65-128">В тексте запроса добавьте представление объекта Ролескопетагаутоассигнмент в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c2d65-128">In the request body, supply a JSON representation for the roleScopeTagAutoAssignment object.</span></span>

<span data-ttu-id="c2d65-129">В следующей таблице приведены свойства, необходимые при создании Ролескопетагаутоассигнмент.</span><span class="sxs-lookup"><span data-stu-id="c2d65-129">The following table shows the properties that are required when you create the roleScopeTagAutoAssignment.</span></span>

|<span data-ttu-id="c2d65-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c2d65-130">Property</span></span>|<span data-ttu-id="c2d65-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c2d65-131">Type</span></span>|<span data-ttu-id="c2d65-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c2d65-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2d65-133">id</span><span class="sxs-lookup"><span data-stu-id="c2d65-133">id</span></span>|<span data-ttu-id="c2d65-134">String</span><span class="sxs-lookup"><span data-stu-id="c2d65-134">String</span></span>|<span data-ttu-id="c2d65-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c2d65-135">Key of the entity.</span></span>|
|<span data-ttu-id="c2d65-136">target</span><span class="sxs-lookup"><span data-stu-id="c2d65-136">target</span></span>|[<span data-ttu-id="c2d65-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="c2d65-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="c2d65-138">Целевой объект автоматического назначения для определенного тега области применения роли.</span><span class="sxs-lookup"><span data-stu-id="c2d65-138">The auto-assignment target for the specific Role Scope Tag.</span></span>|



## <a name="response"></a><span data-ttu-id="c2d65-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="c2d65-139">Response</span></span>
<span data-ttu-id="c2d65-140">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [ролескопетагаутоассигнмент](../resources/intune-rbac-rolescopetagautoassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c2d65-140">If successful, this method returns a `201 Created` response code and a [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2d65-141">Пример</span><span class="sxs-lookup"><span data-stu-id="c2d65-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="c2d65-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="c2d65-142">Request</span></span>
<span data-ttu-id="c2d65-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c2d65-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}/assignments
Content-type: application/json
Content-length: 166

{
  "@odata.type": "#microsoft.graph.roleScopeTagAutoAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="c2d65-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2d65-144">Response</span></span>
<span data-ttu-id="c2d65-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c2d65-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



