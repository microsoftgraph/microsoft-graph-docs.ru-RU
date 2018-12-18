---
title: Перечисление объектов resourceOperation
description: Список свойств и связей объектов resourceOperation.
author: tfitzmac
ms.openlocfilehash: af691d9f0563fa3b9805a512f234b35d1bad4d74
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319196"
---
# <a name="list-resourceoperations"></a><span data-ttu-id="e766a-103">Перечисление объектов resourceOperation</span><span class="sxs-lookup"><span data-stu-id="e766a-103">List resourceOperations</span></span>

> <span data-ttu-id="e766a-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e766a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e766a-105">Список свойств и связей объектов [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="e766a-105">List properties and relationships of the [resourceOperation](../resources/intune-rbac-resourceoperation.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e766a-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e766a-106">Prerequisites</span></span>
<span data-ttu-id="e766a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e766a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e766a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e766a-109">Permission type</span></span>|<span data-ttu-id="e766a-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e766a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e766a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e766a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e766a-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="e766a-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="e766a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e766a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e766a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e766a-114">Not supported.</span></span>|
|<span data-ttu-id="e766a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e766a-115">Application</span></span>|<span data-ttu-id="e766a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e766a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e766a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e766a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/resourceOperations
```

## <a name="request-headers"></a><span data-ttu-id="e766a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e766a-118">Request headers</span></span>
|<span data-ttu-id="e766a-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e766a-119">Header</span></span>|<span data-ttu-id="e766a-120">Значение</span><span class="sxs-lookup"><span data-stu-id="e766a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e766a-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e766a-121">Authorization</span></span>|<span data-ttu-id="e766a-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e766a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e766a-123">Accept</span><span class="sxs-lookup"><span data-stu-id="e766a-123">Accept</span></span>|<span data-ttu-id="e766a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e766a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e766a-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e766a-125">Request body</span></span>
<span data-ttu-id="e766a-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e766a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e766a-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="e766a-127">Response</span></span>
<span data-ttu-id="e766a-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [resourceOperation](../resources/intune-rbac-resourceoperation.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e766a-128">If successful, this method returns a `200 OK` response code and a collection of [resourceOperation](../resources/intune-rbac-resourceoperation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e766a-129">Пример</span><span class="sxs-lookup"><span data-stu-id="e766a-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="e766a-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="e766a-130">Request</span></span>
<span data-ttu-id="e766a-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e766a-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/resourceOperations
```

### <a name="response"></a><span data-ttu-id="e766a-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="e766a-132">Response</span></span>
<span data-ttu-id="e766a-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e766a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 280

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.resourceOperation",
      "id": "232b8fee-8fee-232b-ee8f-2b23ee8f2b23",
      "resourceName": "Resource Name value",
      "actionName": "Action Name value",
      "description": "Description value"
    }
  ]
}
```



