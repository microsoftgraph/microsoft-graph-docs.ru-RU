---
title: Получение объекта resourceOperation
description: Чтение свойств и связей объекта resourceOperation.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 80345f5ed9f6675f63882104fc983c0dc6586191
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43461331"
---
# <a name="get-resourceoperation"></a><span data-ttu-id="978e2-103">Получение объекта resourceOperation</span><span class="sxs-lookup"><span data-stu-id="978e2-103">Get resourceOperation</span></span>

<span data-ttu-id="978e2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="978e2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="978e2-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="978e2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="978e2-106">Чтение свойств и связей объекта [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="978e2-106">Read properties and relationships of the [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="978e2-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="978e2-107">Prerequisites</span></span>
<span data-ttu-id="978e2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="978e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="978e2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="978e2-110">Permission type</span></span>|<span data-ttu-id="978e2-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="978e2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="978e2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="978e2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="978e2-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="978e2-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="978e2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="978e2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="978e2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="978e2-115">Not supported.</span></span>|
|<span data-ttu-id="978e2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="978e2-116">Application</span></span>|<span data-ttu-id="978e2-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="978e2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="978e2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="978e2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/resourceOperations/{resourceOperationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="978e2-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="978e2-119">Optional query parameters</span></span>
<span data-ttu-id="978e2-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="978e2-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="978e2-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="978e2-121">Request headers</span></span>
|<span data-ttu-id="978e2-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="978e2-122">Header</span></span>|<span data-ttu-id="978e2-123">Значение</span><span class="sxs-lookup"><span data-stu-id="978e2-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="978e2-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="978e2-124">Authorization</span></span>|<span data-ttu-id="978e2-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="978e2-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="978e2-126">Accept</span><span class="sxs-lookup"><span data-stu-id="978e2-126">Accept</span></span>|<span data-ttu-id="978e2-127">application/json</span><span class="sxs-lookup"><span data-stu-id="978e2-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="978e2-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="978e2-128">Request body</span></span>
<span data-ttu-id="978e2-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="978e2-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="978e2-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="978e2-130">Response</span></span>
<span data-ttu-id="978e2-131">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [resourceOperation](../resources/intune-rbac-resourceoperation.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="978e2-131">If successful, this method returns a `200 OK` response code and [resourceOperation](../resources/intune-rbac-resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="978e2-132">Пример</span><span class="sxs-lookup"><span data-stu-id="978e2-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="978e2-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="978e2-133">Request</span></span>
<span data-ttu-id="978e2-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="978e2-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/resourceOperations/{resourceOperationId}
```

### <a name="response"></a><span data-ttu-id="978e2-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="978e2-135">Response</span></span>
<span data-ttu-id="978e2-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="978e2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 256

{
  "value": {
    "@odata.type": "#microsoft.graph.resourceOperation",
    "id": "232b8fee-8fee-232b-ee8f-2b23ee8f2b23",
    "resourceName": "Resource Name value",
    "actionName": "Action Name value",
    "description": "Description value"
  }
}
```






