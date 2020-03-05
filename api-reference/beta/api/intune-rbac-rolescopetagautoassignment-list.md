---
title: Список Ролескопетагаутоассигнментс
description: Список свойств и связей объектов Ролескопетагаутоассигнмент.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8fc567f51883e92a565f8d2880566cd32463a911
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42459367"
---
# <a name="list-rolescopetagautoassignments"></a><span data-ttu-id="aef98-103">Список Ролескопетагаутоассигнментс</span><span class="sxs-lookup"><span data-stu-id="aef98-103">List roleScopeTagAutoAssignments</span></span>

<span data-ttu-id="aef98-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="aef98-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aef98-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aef98-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aef98-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="aef98-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aef98-107">Список свойств и связей объектов [ролескопетагаутоассигнмент](../resources/intune-rbac-rolescopetagautoassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="aef98-107">List properties and relationships of the [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aef98-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="aef98-108">Prerequisites</span></span>
<span data-ttu-id="aef98-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aef98-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aef98-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aef98-111">Permission type</span></span>|<span data-ttu-id="aef98-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="aef98-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aef98-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aef98-113">Delegated (work or school account)</span></span>|<span data-ttu-id="aef98-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="aef98-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="aef98-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aef98-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aef98-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aef98-116">Not supported.</span></span>|
|<span data-ttu-id="aef98-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aef98-117">Application</span></span>|<span data-ttu-id="aef98-118">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="aef98-118">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="aef98-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aef98-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="aef98-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="aef98-120">Request headers</span></span>
|<span data-ttu-id="aef98-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="aef98-121">Header</span></span>|<span data-ttu-id="aef98-122">Значение</span><span class="sxs-lookup"><span data-stu-id="aef98-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aef98-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="aef98-123">Authorization</span></span>|<span data-ttu-id="aef98-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aef98-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aef98-125">Accept</span><span class="sxs-lookup"><span data-stu-id="aef98-125">Accept</span></span>|<span data-ttu-id="aef98-126">application/json</span><span class="sxs-lookup"><span data-stu-id="aef98-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aef98-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="aef98-127">Request body</span></span>
<span data-ttu-id="aef98-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="aef98-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aef98-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="aef98-129">Response</span></span>
<span data-ttu-id="aef98-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [ролескопетагаутоассигнмент](../resources/intune-rbac-rolescopetagautoassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="aef98-130">If successful, this method returns a `200 OK` response code and a collection of [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aef98-131">Пример</span><span class="sxs-lookup"><span data-stu-id="aef98-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="aef98-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="aef98-132">Request</span></span>
<span data-ttu-id="aef98-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aef98-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}/assignments
```

### <a name="response"></a><span data-ttu-id="aef98-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="aef98-134">Response</span></span>
<span data-ttu-id="aef98-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="aef98-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 268

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.roleScopeTagAutoAssignment",
      "id": "256e6375-6375-256e-7563-6e2575636e25",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```





