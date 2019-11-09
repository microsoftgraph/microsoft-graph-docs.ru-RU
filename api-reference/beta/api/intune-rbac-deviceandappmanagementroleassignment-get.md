---
title: Получение объекта deviceAndAppManagementRoleAssignment
description: Чтение свойств и связей объекта deviceAndAppManagementRoleAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d804807a0208e547d50fc5375acaa0c3745289af
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/09/2019
ms.locfileid: "38086419"
---
# <a name="get-deviceandappmanagementroleassignment"></a><span data-ttu-id="20778-103">Получение объекта deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="20778-103">Get deviceAndAppManagementRoleAssignment</span></span>

> <span data-ttu-id="20778-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20778-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="20778-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="20778-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="20778-106">Чтение свойств и связей объекта [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="20778-106">Read properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="20778-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="20778-107">Prerequisites</span></span>
<span data-ttu-id="20778-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20778-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20778-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="20778-110">Permission type</span></span>|<span data-ttu-id="20778-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="20778-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="20778-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="20778-112">Delegated (work or school account)</span></span>|<span data-ttu-id="20778-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="20778-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="20778-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="20778-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="20778-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20778-115">Not supported.</span></span>|
|<span data-ttu-id="20778-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="20778-116">Application</span></span>|<span data-ttu-id="20778-117">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="20778-117">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="20778-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="20778-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="20778-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="20778-119">Optional query parameters</span></span>
<span data-ttu-id="20778-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="20778-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="20778-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="20778-121">Request headers</span></span>
|<span data-ttu-id="20778-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="20778-122">Header</span></span>|<span data-ttu-id="20778-123">Значение</span><span class="sxs-lookup"><span data-stu-id="20778-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="20778-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="20778-124">Authorization</span></span>|<span data-ttu-id="20778-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="20778-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="20778-126">Accept</span><span class="sxs-lookup"><span data-stu-id="20778-126">Accept</span></span>|<span data-ttu-id="20778-127">application/json</span><span class="sxs-lookup"><span data-stu-id="20778-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="20778-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="20778-128">Request body</span></span>
<span data-ttu-id="20778-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="20778-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="20778-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="20778-130">Response</span></span>
<span data-ttu-id="20778-131">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="20778-131">If successful, this method returns a `200 OK` response code and [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20778-132">Пример</span><span class="sxs-lookup"><span data-stu-id="20778-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="20778-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="20778-133">Request</span></span>
<span data-ttu-id="20778-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="20778-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

### <a name="response"></a><span data-ttu-id="20778-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="20778-135">Response</span></span>
<span data-ttu-id="20778-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="20778-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 438

{
  "value": {
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
}
```






