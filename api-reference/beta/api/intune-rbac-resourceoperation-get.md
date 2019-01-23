---
title: Получение объекта resourceOperation
description: Чтение свойств и связей объекта resourceOperation.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: da1c9b49771fe9cea08aa40004332a7374ce8577
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421860"
---
# <a name="get-resourceoperation"></a><span data-ttu-id="82317-103">Получение объекта resourceOperation</span><span class="sxs-lookup"><span data-stu-id="82317-103">Get resourceOperation</span></span>

> <span data-ttu-id="82317-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="82317-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="82317-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82317-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="82317-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="82317-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82317-107">Чтение свойств и связей объекта [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="82317-107">Read properties and relationships of the [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="82317-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="82317-108">Prerequisites</span></span>
<span data-ttu-id="82317-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="82317-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="82317-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="82317-111">Permission type</span></span>|<span data-ttu-id="82317-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="82317-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82317-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="82317-113">Delegated (work or school account)</span></span>|<span data-ttu-id="82317-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="82317-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="82317-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="82317-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82317-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82317-116">Not supported.</span></span>|
|<span data-ttu-id="82317-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="82317-117">Application</span></span>|<span data-ttu-id="82317-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82317-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="82317-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="82317-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/resourceOperations/{resourceOperationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="82317-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="82317-120">Optional query parameters</span></span>
<span data-ttu-id="82317-121">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="82317-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="82317-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="82317-122">Request headers</span></span>
|<span data-ttu-id="82317-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="82317-123">Header</span></span>|<span data-ttu-id="82317-124">Значение</span><span class="sxs-lookup"><span data-stu-id="82317-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="82317-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="82317-125">Authorization</span></span>|<span data-ttu-id="82317-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="82317-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="82317-127">Accept</span><span class="sxs-lookup"><span data-stu-id="82317-127">Accept</span></span>|<span data-ttu-id="82317-128">application/json</span><span class="sxs-lookup"><span data-stu-id="82317-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="82317-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="82317-129">Request body</span></span>
<span data-ttu-id="82317-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="82317-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="82317-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="82317-131">Response</span></span>
<span data-ttu-id="82317-132">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [resourceOperation](../resources/intune-rbac-resourceoperation.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="82317-132">If successful, this method returns a `200 OK` response code and [resourceOperation](../resources/intune-rbac-resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82317-133">Пример</span><span class="sxs-lookup"><span data-stu-id="82317-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="82317-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="82317-134">Request</span></span>
<span data-ttu-id="82317-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="82317-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/resourceOperations/{resourceOperationId}
```

### <a name="response"></a><span data-ttu-id="82317-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="82317-136">Response</span></span>
<span data-ttu-id="82317-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="82317-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 331

{
  "value": {
    "@odata.type": "#microsoft.graph.resourceOperation",
    "id": "232b8fee-8fee-232b-ee8f-2b23ee8f2b23",
    "resource": "Resource value",
    "resourceName": "Resource Name value",
    "actionName": "Action Name value",
    "description": "Description value",
    "enabledForScopeValidation": true
  }
}
```




