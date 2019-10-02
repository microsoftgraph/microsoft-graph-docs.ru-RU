---
title: Get roleAssignment
description: Чтение свойств и связей объекта roleAssignment.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 47f63372ffac69c4c8c2a84b07e09935f1ea933b
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37361807"
---
# <a name="get-roleassignment"></a><span data-ttu-id="e27bf-103">Get roleAssignment</span><span class="sxs-lookup"><span data-stu-id="e27bf-103">Get roleAssignment</span></span>

> <span data-ttu-id="e27bf-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e27bf-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e27bf-105">Чтение свойств и связей объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e27bf-105">Read properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e27bf-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="e27bf-106">Prerequisites</span></span>
<span data-ttu-id="e27bf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e27bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e27bf-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e27bf-109">Permission type</span></span>|<span data-ttu-id="e27bf-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e27bf-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e27bf-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e27bf-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e27bf-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="e27bf-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="e27bf-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e27bf-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e27bf-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e27bf-114">Not supported.</span></span>|
|<span data-ttu-id="e27bf-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e27bf-115">Application</span></span>|<span data-ttu-id="e27bf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e27bf-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e27bf-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e27bf-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e27bf-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e27bf-118">Optional query parameters</span></span>
<span data-ttu-id="e27bf-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e27bf-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e27bf-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e27bf-120">Request headers</span></span>
|<span data-ttu-id="e27bf-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e27bf-121">Header</span></span>|<span data-ttu-id="e27bf-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e27bf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e27bf-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e27bf-123">Authorization</span></span>|<span data-ttu-id="e27bf-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e27bf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e27bf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e27bf-125">Accept</span></span>|<span data-ttu-id="e27bf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e27bf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e27bf-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e27bf-127">Request body</span></span>
<span data-ttu-id="e27bf-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e27bf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e27bf-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="e27bf-129">Response</span></span>
<span data-ttu-id="e27bf-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [roleAssignment](../resources/intune-rbac-roleassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e27bf-130">If successful, this method returns a `200 OK` response code and [roleAssignment](../resources/intune-rbac-roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e27bf-131">Пример</span><span class="sxs-lookup"><span data-stu-id="e27bf-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e27bf-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e27bf-132">Request</span></span>
<span data-ttu-id="e27bf-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e27bf-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
```

### <a name="response"></a><span data-ttu-id="e27bf-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="e27bf-134">Response</span></span>
<span data-ttu-id="e27bf-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e27bf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 275

{
  "value": {
    "@odata.type": "#microsoft.graph.roleAssignment",
    "id": "b3234d24-4d24-b323-244d-23b3244d23b3",
    "displayName": "Display Name value",
    "description": "Description value",
    "resourceScopes": [
      "Resource Scopes value"
    ]
  }
}
```




