---
title: Получение объекта deviceAndAppManagementRoleAssignment
description: Чтение свойств и связей объекта deviceAndAppManagementRoleAssignment.
ms.openlocfilehash: 9791019c586b322c96506059ab36bc7c6705c980
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026044"
---
# <a name="get-deviceandappmanagementroleassignment"></a><span data-ttu-id="52924-103">Получение объекта deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="52924-103">Get deviceAndAppManagementRoleAssignment</span></span>

> <span data-ttu-id="52924-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="52924-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="52924-105">Чтение свойств и связей объекта [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="52924-105">Read properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="52924-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="52924-106">Prerequisites</span></span>
<span data-ttu-id="52924-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52924-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52924-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="52924-109">Permission type</span></span>|<span data-ttu-id="52924-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="52924-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="52924-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="52924-111">Delegated (work or school account)</span></span>|<span data-ttu-id="52924-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="52924-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="52924-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="52924-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="52924-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52924-114">Not supported.</span></span>|
|<span data-ttu-id="52924-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="52924-115">Application</span></span>|<span data-ttu-id="52924-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52924-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="52924-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="52924-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="52924-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="52924-118">Optional query parameters</span></span>
<span data-ttu-id="52924-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="52924-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="52924-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="52924-120">Request headers</span></span>
|<span data-ttu-id="52924-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="52924-121">Header</span></span>|<span data-ttu-id="52924-122">Значение</span><span class="sxs-lookup"><span data-stu-id="52924-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="52924-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="52924-123">Authorization</span></span>|<span data-ttu-id="52924-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="52924-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="52924-125">Accept</span><span class="sxs-lookup"><span data-stu-id="52924-125">Accept</span></span>|<span data-ttu-id="52924-126">application/json</span><span class="sxs-lookup"><span data-stu-id="52924-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="52924-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="52924-127">Request body</span></span>
<span data-ttu-id="52924-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="52924-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="52924-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="52924-129">Response</span></span>
<span data-ttu-id="52924-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="52924-130">If successful, this method returns a `200 OK` response code and [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52924-131">Пример</span><span class="sxs-lookup"><span data-stu-id="52924-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="52924-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="52924-132">Request</span></span>
<span data-ttu-id="52924-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="52924-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

### <a name="response"></a><span data-ttu-id="52924-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="52924-134">Response</span></span>
<span data-ttu-id="52924-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="52924-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



