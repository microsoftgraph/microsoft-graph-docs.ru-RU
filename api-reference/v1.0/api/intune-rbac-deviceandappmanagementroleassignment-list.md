---
title: Перечисление объектов deviceAndAppManagementRoleAssignment
description: Список свойств и связей объектов deviceAndAppManagementRoleAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 199794d8971214577b1a5e64e4b890aa643d60b8
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30989528"
---
# <a name="list-deviceandappmanagementroleassignments"></a><span data-ttu-id="a0bbb-103">Перечисление объектов deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="a0bbb-103">List deviceAndAppManagementRoleAssignments</span></span>

> <span data-ttu-id="a0bbb-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a0bbb-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0bbb-105">Список свойств и связей объектов [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a0bbb-105">List properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a0bbb-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a0bbb-106">Prerequisites</span></span>
<span data-ttu-id="a0bbb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0bbb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0bbb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a0bbb-109">Permission type</span></span>|<span data-ttu-id="a0bbb-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a0bbb-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0bbb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a0bbb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a0bbb-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="a0bbb-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="a0bbb-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a0bbb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0bbb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0bbb-114">Not supported.</span></span>|
|<span data-ttu-id="a0bbb-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a0bbb-115">Application</span></span>|<span data-ttu-id="a0bbb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0bbb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0bbb-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a0bbb-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="a0bbb-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a0bbb-118">Request headers</span></span>
|<span data-ttu-id="a0bbb-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a0bbb-119">Header</span></span>|<span data-ttu-id="a0bbb-120">Значение</span><span class="sxs-lookup"><span data-stu-id="a0bbb-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a0bbb-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a0bbb-121">Authorization</span></span>|<span data-ttu-id="a0bbb-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a0bbb-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a0bbb-123">Accept</span><span class="sxs-lookup"><span data-stu-id="a0bbb-123">Accept</span></span>|<span data-ttu-id="a0bbb-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a0bbb-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0bbb-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a0bbb-125">Request body</span></span>
<span data-ttu-id="a0bbb-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a0bbb-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a0bbb-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="a0bbb-127">Response</span></span>
<span data-ttu-id="a0bbb-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a0bbb-128">If successful, this method returns a `200 OK` response code and a collection of [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0bbb-129">Пример</span><span class="sxs-lookup"><span data-stu-id="a0bbb-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="a0bbb-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="a0bbb-130">Request</span></span>
<span data-ttu-id="a0bbb-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a0bbb-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/roleAssignments
```

### <a name="response"></a><span data-ttu-id="a0bbb-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="a0bbb-132">Response</span></span>
<span data-ttu-id="a0bbb-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a0bbb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



