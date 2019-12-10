---
title: Перечисление объектов deviceAndAppManagementRoleAssignment
description: Список свойств и связей объектов deviceAndAppManagementRoleAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f7bfdc20bee075801b2eec4b2f923b75033d4761
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39940723"
---
# <a name="list-deviceandappmanagementroleassignments"></a><span data-ttu-id="c5a50-103">Перечисление объектов deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="c5a50-103">List deviceAndAppManagementRoleAssignments</span></span>

> <span data-ttu-id="c5a50-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5a50-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c5a50-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c5a50-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5a50-106">Список свойств и связей объектов [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c5a50-106">List properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c5a50-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c5a50-107">Prerequisites</span></span>
<span data-ttu-id="c5a50-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5a50-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5a50-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c5a50-110">Permission type</span></span>|<span data-ttu-id="c5a50-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c5a50-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5a50-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c5a50-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c5a50-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="c5a50-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="c5a50-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c5a50-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5a50-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5a50-115">Not supported.</span></span>|
|<span data-ttu-id="c5a50-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c5a50-116">Application</span></span>|<span data-ttu-id="c5a50-117">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="c5a50-117">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5a50-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c5a50-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="c5a50-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c5a50-119">Request headers</span></span>
|<span data-ttu-id="c5a50-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c5a50-120">Header</span></span>|<span data-ttu-id="c5a50-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c5a50-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c5a50-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c5a50-122">Authorization</span></span>|<span data-ttu-id="c5a50-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c5a50-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c5a50-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c5a50-124">Accept</span></span>|<span data-ttu-id="c5a50-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c5a50-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5a50-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c5a50-126">Request body</span></span>
<span data-ttu-id="c5a50-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c5a50-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c5a50-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="c5a50-128">Response</span></span>
<span data-ttu-id="c5a50-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c5a50-129">If successful, this method returns a `200 OK` response code and a collection of [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5a50-130">Пример</span><span class="sxs-lookup"><span data-stu-id="c5a50-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="c5a50-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="c5a50-131">Request</span></span>
<span data-ttu-id="c5a50-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c5a50-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleAssignments
```

### <a name="response"></a><span data-ttu-id="c5a50-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5a50-133">Response</span></span>
<span data-ttu-id="c5a50-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c5a50-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





