---
title: Получение объекта deviceAndAppManagementRoleAssignment
description: Чтение свойств и связей объекта deviceAndAppManagementRoleAssignment.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b7a9e0772861cebf2c4d5237fe8584ba1349f445
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37362003"
---
# <a name="get-deviceandappmanagementroleassignment"></a><span data-ttu-id="abbb5-103">Получение объекта deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="abbb5-103">Get deviceAndAppManagementRoleAssignment</span></span>

> <span data-ttu-id="abbb5-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="abbb5-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="abbb5-105">Чтение свойств и связей объекта [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="abbb5-105">Read properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="abbb5-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="abbb5-106">Prerequisites</span></span>
<span data-ttu-id="abbb5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="abbb5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="abbb5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="abbb5-109">Permission type</span></span>|<span data-ttu-id="abbb5-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="abbb5-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="abbb5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="abbb5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="abbb5-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="abbb5-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="abbb5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="abbb5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="abbb5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="abbb5-114">Not supported.</span></span>|
|<span data-ttu-id="abbb5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="abbb5-115">Application</span></span>|<span data-ttu-id="abbb5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="abbb5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="abbb5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="abbb5-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="abbb5-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="abbb5-118">Optional query parameters</span></span>
<span data-ttu-id="abbb5-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="abbb5-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="abbb5-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="abbb5-120">Request headers</span></span>
|<span data-ttu-id="abbb5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="abbb5-121">Header</span></span>|<span data-ttu-id="abbb5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="abbb5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="abbb5-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="abbb5-123">Authorization</span></span>|<span data-ttu-id="abbb5-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="abbb5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="abbb5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="abbb5-125">Accept</span></span>|<span data-ttu-id="abbb5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="abbb5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="abbb5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="abbb5-127">Request body</span></span>
<span data-ttu-id="abbb5-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="abbb5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="abbb5-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="abbb5-129">Response</span></span>
<span data-ttu-id="abbb5-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="abbb5-130">If successful, this method returns a `200 OK` response code and [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="abbb5-131">Пример</span><span class="sxs-lookup"><span data-stu-id="abbb5-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="abbb5-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="abbb5-132">Request</span></span>
<span data-ttu-id="abbb5-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="abbb5-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

### <a name="response"></a><span data-ttu-id="abbb5-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="abbb5-134">Response</span></span>
<span data-ttu-id="abbb5-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="abbb5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




