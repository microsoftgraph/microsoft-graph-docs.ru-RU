---
title: Перечисление объектов deviceAndAppManagementRoleAssignment
description: Список свойств и связей объектов deviceAndAppManagementRoleAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fad79e94b0e40e549429b5fb6265e4f2acd04a78
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48709107"
---
# <a name="list-deviceandappmanagementroleassignments"></a><span data-ttu-id="aba28-103">Перечисление объектов deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="aba28-103">List deviceAndAppManagementRoleAssignments</span></span>

<span data-ttu-id="aba28-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aba28-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aba28-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aba28-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aba28-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="aba28-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aba28-107">Список свойств и связей объектов [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="aba28-107">List properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aba28-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="aba28-108">Prerequisites</span></span>
<span data-ttu-id="aba28-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aba28-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aba28-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aba28-111">Permission type</span></span>|<span data-ttu-id="aba28-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="aba28-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aba28-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aba28-113">Delegated (work or school account)</span></span>|<span data-ttu-id="aba28-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="aba28-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="aba28-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aba28-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aba28-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aba28-116">Not supported.</span></span>|
|<span data-ttu-id="aba28-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aba28-117">Application</span></span>|<span data-ttu-id="aba28-118">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="aba28-118">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="aba28-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aba28-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="aba28-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="aba28-120">Request headers</span></span>
|<span data-ttu-id="aba28-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="aba28-121">Header</span></span>|<span data-ttu-id="aba28-122">Значение</span><span class="sxs-lookup"><span data-stu-id="aba28-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aba28-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="aba28-123">Authorization</span></span>|<span data-ttu-id="aba28-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aba28-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aba28-125">Accept</span><span class="sxs-lookup"><span data-stu-id="aba28-125">Accept</span></span>|<span data-ttu-id="aba28-126">application/json</span><span class="sxs-lookup"><span data-stu-id="aba28-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aba28-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="aba28-127">Request body</span></span>
<span data-ttu-id="aba28-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="aba28-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aba28-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="aba28-129">Response</span></span>
<span data-ttu-id="aba28-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="aba28-130">If successful, this method returns a `200 OK` response code and a collection of [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aba28-131">Пример</span><span class="sxs-lookup"><span data-stu-id="aba28-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="aba28-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="aba28-132">Request</span></span>
<span data-ttu-id="aba28-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aba28-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleAssignments
```

### <a name="response"></a><span data-ttu-id="aba28-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="aba28-134">Response</span></span>
<span data-ttu-id="aba28-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="aba28-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





