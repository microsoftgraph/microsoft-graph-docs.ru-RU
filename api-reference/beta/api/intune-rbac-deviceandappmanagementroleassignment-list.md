---
title: Перечисление объектов deviceAndAppManagementRoleAssignment
description: Список свойств и связей объектов deviceAndAppManagementRoleAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 74d33333607d8e0bd927127f4575046e4f3ff499
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51158502"
---
# <a name="list-deviceandappmanagementroleassignments"></a><span data-ttu-id="31f96-103">Перечисление объектов deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="31f96-103">List deviceAndAppManagementRoleAssignments</span></span>

<span data-ttu-id="31f96-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31f96-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="31f96-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31f96-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="31f96-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="31f96-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="31f96-107">Список свойств и связей объектов [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="31f96-107">List properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="31f96-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="31f96-108">Prerequisites</span></span>
<span data-ttu-id="31f96-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31f96-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31f96-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="31f96-111">Permission type</span></span>|<span data-ttu-id="31f96-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="31f96-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="31f96-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="31f96-113">Delegated (work or school account)</span></span>|<span data-ttu-id="31f96-114">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31f96-114">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="31f96-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="31f96-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="31f96-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31f96-116">Not supported.</span></span>|
|<span data-ttu-id="31f96-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="31f96-117">Application</span></span>|<span data-ttu-id="31f96-118">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31f96-118">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="31f96-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="31f96-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="31f96-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="31f96-120">Request headers</span></span>
|<span data-ttu-id="31f96-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="31f96-121">Header</span></span>|<span data-ttu-id="31f96-122">Значение</span><span class="sxs-lookup"><span data-stu-id="31f96-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="31f96-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="31f96-123">Authorization</span></span>|<span data-ttu-id="31f96-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="31f96-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="31f96-125">Accept</span><span class="sxs-lookup"><span data-stu-id="31f96-125">Accept</span></span>|<span data-ttu-id="31f96-126">application/json</span><span class="sxs-lookup"><span data-stu-id="31f96-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="31f96-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="31f96-127">Request body</span></span>
<span data-ttu-id="31f96-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="31f96-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="31f96-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="31f96-129">Response</span></span>
<span data-ttu-id="31f96-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="31f96-130">If successful, this method returns a `200 OK` response code and a collection of [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31f96-131">Пример</span><span class="sxs-lookup"><span data-stu-id="31f96-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="31f96-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="31f96-132">Request</span></span>
<span data-ttu-id="31f96-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="31f96-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleAssignments
```

### <a name="response"></a><span data-ttu-id="31f96-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="31f96-134">Response</span></span>
<span data-ttu-id="31f96-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="31f96-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 480

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
      "id": "a12e8ebb-8ebb-a12e-bb8e-2ea1bb8e2ea1",
      "displayName": "Display Name value",
      "description": "Description value",
      "scopeMembers": [
        "Scope Members value"
      ],
      "scopeType": "allDevices",
      "resourceScopes": [
        "Resource Scopes value"
      ],
      "members": [
        "Members value"
      ]
    }
  ]
}
```




