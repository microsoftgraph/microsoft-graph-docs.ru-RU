---
title: List roleScopeTagAutoAssignments
description: Список свойств и связей объектов roleScopeTagAutoAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 08bcae600d3657566eb2a1ff0d6c6dd387d7e852
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51134482"
---
# <a name="list-rolescopetagautoassignments"></a><span data-ttu-id="23ff7-103">List roleScopeTagAutoAssignments</span><span class="sxs-lookup"><span data-stu-id="23ff7-103">List roleScopeTagAutoAssignments</span></span>

<span data-ttu-id="23ff7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23ff7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="23ff7-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23ff7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="23ff7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="23ff7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23ff7-107">Список свойств и связей объектов [roleScopeTagAutoAssignment.](../resources/intune-rbac-rolescopetagautoassignment.md)</span><span class="sxs-lookup"><span data-stu-id="23ff7-107">List properties and relationships of the [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="23ff7-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="23ff7-108">Prerequisites</span></span>
<span data-ttu-id="23ff7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23ff7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23ff7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="23ff7-111">Permission type</span></span>|<span data-ttu-id="23ff7-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="23ff7-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="23ff7-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="23ff7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="23ff7-114">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23ff7-114">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="23ff7-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="23ff7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="23ff7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23ff7-116">Not supported.</span></span>|
|<span data-ttu-id="23ff7-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="23ff7-117">Application</span></span>|<span data-ttu-id="23ff7-118">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23ff7-118">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="23ff7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="23ff7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="23ff7-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="23ff7-120">Request headers</span></span>
|<span data-ttu-id="23ff7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="23ff7-121">Header</span></span>|<span data-ttu-id="23ff7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="23ff7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="23ff7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="23ff7-123">Authorization</span></span>|<span data-ttu-id="23ff7-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="23ff7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="23ff7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="23ff7-125">Accept</span></span>|<span data-ttu-id="23ff7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="23ff7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="23ff7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="23ff7-127">Request body</span></span>
<span data-ttu-id="23ff7-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="23ff7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="23ff7-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="23ff7-129">Response</span></span>
<span data-ttu-id="23ff7-130">В случае успешного выполнения этот метод возвращает код ответа и коллекцию объектов `200 OK` [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="23ff7-130">If successful, this method returns a `200 OK` response code and a collection of [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23ff7-131">Пример</span><span class="sxs-lookup"><span data-stu-id="23ff7-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="23ff7-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="23ff7-132">Request</span></span>
<span data-ttu-id="23ff7-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="23ff7-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}/assignments
```

### <a name="response"></a><span data-ttu-id="23ff7-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="23ff7-134">Response</span></span>
<span data-ttu-id="23ff7-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="23ff7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 499

{
  "value": [
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
  ]
}
```




