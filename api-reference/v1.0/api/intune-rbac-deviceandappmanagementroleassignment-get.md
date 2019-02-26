---
title: Получение объекта deviceAndAppManagementRoleAssignment
description: Чтение свойств и связей объекта deviceAndAppManagementRoleAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 30f534ed4eceb5a4615f4e6f5e3dc0f7cc4375ad
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30256667"
---
# <a name="get-deviceandappmanagementroleassignment"></a><span data-ttu-id="c7a7b-103">Получение объекта deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="c7a7b-103">Get deviceAndAppManagementRoleAssignment</span></span>

> <span data-ttu-id="c7a7b-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c7a7b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7a7b-105">Чтение свойств и связей объекта [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c7a7b-105">Read properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c7a7b-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c7a7b-106">Prerequisites</span></span>
<span data-ttu-id="c7a7b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c7a7b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c7a7b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c7a7b-109">Permission type</span></span>|<span data-ttu-id="c7a7b-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c7a7b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7a7b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c7a7b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c7a7b-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="c7a7b-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="c7a7b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c7a7b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7a7b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7a7b-114">Not supported.</span></span>|
|<span data-ttu-id="c7a7b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c7a7b-115">Application</span></span>|<span data-ttu-id="c7a7b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7a7b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7a7b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c7a7b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c7a7b-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c7a7b-118">Optional query parameters</span></span>
<span data-ttu-id="c7a7b-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c7a7b-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c7a7b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c7a7b-120">Request headers</span></span>
|<span data-ttu-id="c7a7b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c7a7b-121">Header</span></span>|<span data-ttu-id="c7a7b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c7a7b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c7a7b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7a7b-123">Authorization</span></span>|<span data-ttu-id="c7a7b-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c7a7b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c7a7b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c7a7b-125">Accept</span></span>|<span data-ttu-id="c7a7b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c7a7b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7a7b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c7a7b-127">Request body</span></span>
<span data-ttu-id="c7a7b-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c7a7b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c7a7b-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7a7b-129">Response</span></span>
<span data-ttu-id="c7a7b-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c7a7b-130">If successful, this method returns a `200 OK` response code and [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7a7b-131">Пример</span><span class="sxs-lookup"><span data-stu-id="c7a7b-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c7a7b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c7a7b-132">Request</span></span>
<span data-ttu-id="c7a7b-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c7a7b-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

### <a name="response"></a><span data-ttu-id="c7a7b-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="c7a7b-134">Response</span></span>
<span data-ttu-id="c7a7b-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c7a7b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



