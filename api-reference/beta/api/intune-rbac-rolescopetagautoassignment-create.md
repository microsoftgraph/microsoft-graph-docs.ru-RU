---
title: Создание Ролескопетагаутоассигнмент
description: Создание нового объекта Ролескопетагаутоассигнмент.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 46f6e41fb9cdd461ad5fcfe6cd55552618f004ed
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42801560"
---
# <a name="create-rolescopetagautoassignment"></a><span data-ttu-id="4eed2-103">Создание Ролескопетагаутоассигнмент</span><span class="sxs-lookup"><span data-stu-id="4eed2-103">Create roleScopeTagAutoAssignment</span></span>

> <span data-ttu-id="4eed2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4eed2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4eed2-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4eed2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4eed2-106">Создание нового объекта [ролескопетагаутоассигнмент](../resources/intune-rbac-rolescopetagautoassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="4eed2-106">Create a new [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4eed2-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4eed2-107">Prerequisites</span></span>
<span data-ttu-id="4eed2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4eed2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4eed2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4eed2-110">Permission type</span></span>|<span data-ttu-id="4eed2-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4eed2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4eed2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4eed2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4eed2-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4eed2-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="4eed2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4eed2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4eed2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4eed2-115">Not supported.</span></span>|
|<span data-ttu-id="4eed2-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="4eed2-116">Application</span></span>|<span data-ttu-id="4eed2-117">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4eed2-117">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4eed2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4eed2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="4eed2-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4eed2-119">Request headers</span></span>
|<span data-ttu-id="4eed2-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4eed2-120">Header</span></span>|<span data-ttu-id="4eed2-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4eed2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4eed2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4eed2-122">Authorization</span></span>|<span data-ttu-id="4eed2-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4eed2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4eed2-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4eed2-124">Accept</span></span>|<span data-ttu-id="4eed2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4eed2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4eed2-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4eed2-126">Request body</span></span>
<span data-ttu-id="4eed2-127">В тексте запроса добавьте представление объекта Ролескопетагаутоассигнмент в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4eed2-127">In the request body, supply a JSON representation for the roleScopeTagAutoAssignment object.</span></span>

<span data-ttu-id="4eed2-128">В следующей таблице приведены свойства, необходимые при создании Ролескопетагаутоассигнмент.</span><span class="sxs-lookup"><span data-stu-id="4eed2-128">The following table shows the properties that are required when you create the roleScopeTagAutoAssignment.</span></span>

|<span data-ttu-id="4eed2-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="4eed2-129">Property</span></span>|<span data-ttu-id="4eed2-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4eed2-130">Type</span></span>|<span data-ttu-id="4eed2-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4eed2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4eed2-132">id</span><span class="sxs-lookup"><span data-stu-id="4eed2-132">id</span></span>|<span data-ttu-id="4eed2-133">String</span><span class="sxs-lookup"><span data-stu-id="4eed2-133">String</span></span>|<span data-ttu-id="4eed2-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4eed2-134">Key of the entity.</span></span>|
|<span data-ttu-id="4eed2-135">target</span><span class="sxs-lookup"><span data-stu-id="4eed2-135">target</span></span>|[<span data-ttu-id="4eed2-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="4eed2-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="4eed2-137">Целевой объект автоматического назначения для определенного тега области применения роли.</span><span class="sxs-lookup"><span data-stu-id="4eed2-137">The auto-assignment target for the specific Role Scope Tag.</span></span>|



## <a name="response"></a><span data-ttu-id="4eed2-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="4eed2-138">Response</span></span>
<span data-ttu-id="4eed2-139">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [ролескопетагаутоассигнмент](../resources/intune-rbac-rolescopetagautoassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4eed2-139">If successful, this method returns a `201 Created` response code and a [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4eed2-140">Пример</span><span class="sxs-lookup"><span data-stu-id="4eed2-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="4eed2-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="4eed2-141">Request</span></span>
<span data-ttu-id="4eed2-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4eed2-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4eed2-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="4eed2-143">Response</span></span>
<span data-ttu-id="4eed2-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4eed2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




