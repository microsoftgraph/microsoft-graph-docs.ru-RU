---
title: Создание roleScopeTagAutoAssignment
description: Создайте новый объект roleScopeTagAutoAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 498ab9824fac01efab4dae5f3d1418d3d175bfef
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51134538"
---
# <a name="create-rolescopetagautoassignment"></a><span data-ttu-id="d1529-103">Создание roleScopeTagAutoAssignment</span><span class="sxs-lookup"><span data-stu-id="d1529-103">Create roleScopeTagAutoAssignment</span></span>

<span data-ttu-id="d1529-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1529-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d1529-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1529-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d1529-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d1529-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1529-107">Создайте новый [объект roleScopeTagAutoAssignment.](../resources/intune-rbac-rolescopetagautoassignment.md)</span><span class="sxs-lookup"><span data-stu-id="d1529-107">Create a new [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d1529-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d1529-108">Prerequisites</span></span>
<span data-ttu-id="d1529-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1529-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1529-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d1529-111">Permission type</span></span>|<span data-ttu-id="d1529-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d1529-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d1529-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d1529-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d1529-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1529-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="d1529-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d1529-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d1529-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1529-116">Not supported.</span></span>|
|<span data-ttu-id="d1529-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="d1529-117">Application</span></span>|<span data-ttu-id="d1529-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1529-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d1529-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d1529-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="d1529-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d1529-120">Request headers</span></span>
|<span data-ttu-id="d1529-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d1529-121">Header</span></span>|<span data-ttu-id="d1529-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d1529-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d1529-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d1529-123">Authorization</span></span>|<span data-ttu-id="d1529-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d1529-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d1529-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d1529-125">Accept</span></span>|<span data-ttu-id="d1529-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d1529-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1529-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d1529-127">Request body</span></span>
<span data-ttu-id="d1529-128">В теле запроса поставляем представление JSON для объекта roleScopeTagAutoAssignment.</span><span class="sxs-lookup"><span data-stu-id="d1529-128">In the request body, supply a JSON representation for the roleScopeTagAutoAssignment object.</span></span>

<span data-ttu-id="d1529-129">В следующей таблице показаны свойства, необходимые при создании ролиScopeTagAutoAssignment.</span><span class="sxs-lookup"><span data-stu-id="d1529-129">The following table shows the properties that are required when you create the roleScopeTagAutoAssignment.</span></span>

|<span data-ttu-id="d1529-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d1529-130">Property</span></span>|<span data-ttu-id="d1529-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d1529-131">Type</span></span>|<span data-ttu-id="d1529-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d1529-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1529-133">id</span><span class="sxs-lookup"><span data-stu-id="d1529-133">id</span></span>|<span data-ttu-id="d1529-134">Строка</span><span class="sxs-lookup"><span data-stu-id="d1529-134">String</span></span>|<span data-ttu-id="d1529-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d1529-135">Key of the entity.</span></span>|
|<span data-ttu-id="d1529-136">target</span><span class="sxs-lookup"><span data-stu-id="d1529-136">target</span></span>|[<span data-ttu-id="d1529-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d1529-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="d1529-138">Цель автоматического назначения для определенного тега области ролей.</span><span class="sxs-lookup"><span data-stu-id="d1529-138">The auto-assignment target for the specific Role Scope Tag.</span></span>|



## <a name="response"></a><span data-ttu-id="d1529-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1529-139">Response</span></span>
<span data-ttu-id="d1529-140">В случае успешного выполнения этот метод возвращает код ответа и объект `201 Created` [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d1529-140">If successful, this method returns a `201 Created` response code and a [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1529-141">Пример</span><span class="sxs-lookup"><span data-stu-id="d1529-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="d1529-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="d1529-142">Request</span></span>
<span data-ttu-id="d1529-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d1529-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}/assignments
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

### <a name="response"></a><span data-ttu-id="d1529-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1529-144">Response</span></span>
<span data-ttu-id="d1529-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d1529-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




