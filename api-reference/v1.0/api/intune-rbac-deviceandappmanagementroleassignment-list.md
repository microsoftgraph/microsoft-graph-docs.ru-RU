---
title: Перечисление объектов deviceAndAppManagementRoleAssignment
description: Список свойств и связей объектов deviceAndAppManagementRoleAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 01a1c4c76a6340011437d3749abbdf8982d73b65
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756234"
---
# <a name="list-deviceandappmanagementroleassignments"></a><span data-ttu-id="07889-103">Перечисление объектов deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="07889-103">List deviceAndAppManagementRoleAssignments</span></span>

<span data-ttu-id="07889-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07889-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="07889-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="07889-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07889-106">Список свойств и связей объектов [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="07889-106">List properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="07889-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="07889-107">Prerequisites</span></span>
<span data-ttu-id="07889-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07889-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07889-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="07889-110">Permission type</span></span>|<span data-ttu-id="07889-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="07889-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="07889-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="07889-112">Delegated (work or school account)</span></span>|<span data-ttu-id="07889-113">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07889-113">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="07889-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="07889-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="07889-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07889-115">Not supported.</span></span>|
|<span data-ttu-id="07889-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="07889-116">Application</span></span>|<span data-ttu-id="07889-117">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07889-117">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="07889-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="07889-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="07889-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="07889-119">Request headers</span></span>
|<span data-ttu-id="07889-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="07889-120">Header</span></span>|<span data-ttu-id="07889-121">Значение</span><span class="sxs-lookup"><span data-stu-id="07889-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="07889-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="07889-122">Authorization</span></span>|<span data-ttu-id="07889-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="07889-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="07889-124">Accept</span><span class="sxs-lookup"><span data-stu-id="07889-124">Accept</span></span>|<span data-ttu-id="07889-125">application/json</span><span class="sxs-lookup"><span data-stu-id="07889-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="07889-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="07889-126">Request body</span></span>
<span data-ttu-id="07889-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="07889-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="07889-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="07889-128">Response</span></span>
<span data-ttu-id="07889-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="07889-129">If successful, this method returns a `200 OK` response code and a collection of [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07889-130">Пример</span><span class="sxs-lookup"><span data-stu-id="07889-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="07889-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="07889-131">Request</span></span>
<span data-ttu-id="07889-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="07889-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/roleAssignments
```

### <a name="response"></a><span data-ttu-id="07889-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="07889-133">Response</span></span>
<span data-ttu-id="07889-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="07889-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 380

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
      "id": "a12e8ebb-8ebb-a12e-bb8e-2ea1bb8e2ea1",
      "displayName": "Display Name value",
      "description": "Description value",
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




