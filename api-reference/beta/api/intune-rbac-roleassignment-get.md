---
title: Get roleAssignment
description: Чтение свойств и связей объекта roleAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8f39d8226b624ace0aa5f33ce06572b616e23c0c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49210664"
---
# <a name="get-roleassignment"></a><span data-ttu-id="a6e60-103">Get roleAssignment</span><span class="sxs-lookup"><span data-stu-id="a6e60-103">Get roleAssignment</span></span>

<span data-ttu-id="a6e60-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6e60-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a6e60-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6e60-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a6e60-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a6e60-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6e60-107">Чтение свойств и связей объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a6e60-107">Read properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a6e60-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="a6e60-108">Prerequisites</span></span>
<span data-ttu-id="a6e60-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6e60-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6e60-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a6e60-111">Permission type</span></span>|<span data-ttu-id="a6e60-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a6e60-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6e60-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a6e60-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a6e60-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="a6e60-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="a6e60-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a6e60-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6e60-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6e60-116">Not supported.</span></span>|
|<span data-ttu-id="a6e60-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="a6e60-117">Application</span></span>|<span data-ttu-id="a6e60-118">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="a6e60-118">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6e60-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a6e60-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a6e60-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a6e60-120">Optional query parameters</span></span>
<span data-ttu-id="a6e60-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a6e60-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a6e60-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a6e60-122">Request headers</span></span>
|<span data-ttu-id="a6e60-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a6e60-123">Header</span></span>|<span data-ttu-id="a6e60-124">Значение</span><span class="sxs-lookup"><span data-stu-id="a6e60-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6e60-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a6e60-125">Authorization</span></span>|<span data-ttu-id="a6e60-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a6e60-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6e60-127">Accept</span><span class="sxs-lookup"><span data-stu-id="a6e60-127">Accept</span></span>|<span data-ttu-id="a6e60-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a6e60-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6e60-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a6e60-129">Request body</span></span>
<span data-ttu-id="a6e60-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a6e60-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a6e60-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="a6e60-131">Response</span></span>
<span data-ttu-id="a6e60-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [roleAssignment](../resources/intune-rbac-roleassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a6e60-132">If successful, this method returns a `200 OK` response code and [roleAssignment](../resources/intune-rbac-roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6e60-133">Пример</span><span class="sxs-lookup"><span data-stu-id="a6e60-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="a6e60-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="a6e60-134">Request</span></span>
<span data-ttu-id="a6e60-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a6e60-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
```

### <a name="response"></a><span data-ttu-id="a6e60-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="a6e60-136">Response</span></span>
<span data-ttu-id="a6e60-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a6e60-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 367

{
  "value": {
    "@odata.type": "#microsoft.graph.roleAssignment",
    "id": "b3234d24-4d24-b323-244d-23b3244d23b3",
    "displayName": "Display Name value",
    "description": "Description value",
    "scopeMembers": [
      "Scope Members value"
    ],
    "scopeType": "allDevices",
    "resourceScopes": [
      "Resource Scopes value"
    ]
  }
}
```




