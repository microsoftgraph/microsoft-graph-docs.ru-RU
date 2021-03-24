---
title: Удаление roleScopeTagAutoAssignment
description: Удаляет рольScopeTagAutoAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 27ce42f45f1c749933557258a5cc53f8341f5ca5
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51134503"
---
# <a name="delete-rolescopetagautoassignment"></a><span data-ttu-id="f24bf-103">Удаление roleScopeTagAutoAssignment</span><span class="sxs-lookup"><span data-stu-id="f24bf-103">Delete roleScopeTagAutoAssignment</span></span>

<span data-ttu-id="f24bf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f24bf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f24bf-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f24bf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f24bf-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f24bf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f24bf-107">Удаляет [рольScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md).</span><span class="sxs-lookup"><span data-stu-id="f24bf-107">Deletes a [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f24bf-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f24bf-108">Prerequisites</span></span>
<span data-ttu-id="f24bf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f24bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f24bf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f24bf-111">Permission type</span></span>|<span data-ttu-id="f24bf-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f24bf-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f24bf-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f24bf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f24bf-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f24bf-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="f24bf-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f24bf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f24bf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f24bf-116">Not supported.</span></span>|
|<span data-ttu-id="f24bf-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="f24bf-117">Application</span></span>|<span data-ttu-id="f24bf-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f24bf-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f24bf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f24bf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}/assignments/{roleScopeTagAutoAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="f24bf-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f24bf-120">Request headers</span></span>
|<span data-ttu-id="f24bf-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f24bf-121">Header</span></span>|<span data-ttu-id="f24bf-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f24bf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f24bf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f24bf-123">Authorization</span></span>|<span data-ttu-id="f24bf-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f24bf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f24bf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f24bf-125">Accept</span></span>|<span data-ttu-id="f24bf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f24bf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f24bf-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f24bf-127">Request body</span></span>
<span data-ttu-id="f24bf-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f24bf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f24bf-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="f24bf-129">Response</span></span>
<span data-ttu-id="f24bf-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f24bf-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f24bf-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f24bf-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f24bf-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f24bf-132">Request</span></span>
<span data-ttu-id="f24bf-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f24bf-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}/assignments/{roleScopeTagAutoAssignmentId}
```

### <a name="response"></a><span data-ttu-id="f24bf-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="f24bf-134">Response</span></span>
<span data-ttu-id="f24bf-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f24bf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




