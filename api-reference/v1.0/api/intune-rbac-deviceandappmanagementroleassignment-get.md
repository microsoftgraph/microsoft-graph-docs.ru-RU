---
title: Получение объекта deviceAndAppManagementRoleAssignment
description: Чтение свойств и связей объекта deviceAndAppManagementRoleAssignment.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2f8ce024d1b33996ac4d273c85cdc36a25024673
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42512344"
---
# <a name="get-deviceandappmanagementroleassignment"></a><span data-ttu-id="4e455-103">Получение объекта deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="4e455-103">Get deviceAndAppManagementRoleAssignment</span></span>

<span data-ttu-id="4e455-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e455-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4e455-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4e455-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e455-106">Чтение свойств и связей объекта [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="4e455-106">Read properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4e455-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4e455-107">Prerequisites</span></span>
<span data-ttu-id="4e455-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e455-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e455-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4e455-110">Permission type</span></span>|<span data-ttu-id="4e455-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4e455-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e455-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4e455-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4e455-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="4e455-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="4e455-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4e455-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e455-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e455-115">Not supported.</span></span>|
|<span data-ttu-id="4e455-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4e455-116">Application</span></span>|<span data-ttu-id="4e455-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e455-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e455-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4e455-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4e455-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4e455-119">Optional query parameters</span></span>
<span data-ttu-id="4e455-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4e455-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4e455-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4e455-121">Request headers</span></span>
|<span data-ttu-id="4e455-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4e455-122">Header</span></span>|<span data-ttu-id="4e455-123">Значение</span><span class="sxs-lookup"><span data-stu-id="4e455-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4e455-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="4e455-124">Authorization</span></span>|<span data-ttu-id="4e455-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4e455-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4e455-126">Accept</span><span class="sxs-lookup"><span data-stu-id="4e455-126">Accept</span></span>|<span data-ttu-id="4e455-127">application/json</span><span class="sxs-lookup"><span data-stu-id="4e455-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e455-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4e455-128">Request body</span></span>
<span data-ttu-id="4e455-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4e455-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4e455-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="4e455-130">Response</span></span>
<span data-ttu-id="4e455-131">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4e455-131">If successful, this method returns a `200 OK` response code and [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e455-132">Пример</span><span class="sxs-lookup"><span data-stu-id="4e455-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="4e455-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="4e455-133">Request</span></span>
<span data-ttu-id="4e455-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4e455-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

### <a name="response"></a><span data-ttu-id="4e455-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e455-135">Response</span></span>
<span data-ttu-id="4e455-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4e455-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 346

{
  "value": {
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
}
```




