---
title: Список объектов roleAssignment
description: Список свойств и связей объектов roleAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ce54ba485641c74e374e853a3396be16190ee905
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937070"
---
# <a name="list-roleassignments"></a><span data-ttu-id="102d3-103">Список объектов roleAssignment</span><span class="sxs-lookup"><span data-stu-id="102d3-103">List roleAssignments</span></span>

> <span data-ttu-id="102d3-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="102d3-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="102d3-105">Список свойств и связей объектов [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="102d3-105">List properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="102d3-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="102d3-106">Prerequisites</span></span>
<span data-ttu-id="102d3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="102d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="102d3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="102d3-109">Permission type</span></span>|<span data-ttu-id="102d3-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="102d3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="102d3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="102d3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="102d3-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="102d3-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="102d3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="102d3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="102d3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="102d3-114">Not supported.</span></span>|
|<span data-ttu-id="102d3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="102d3-115">Application</span></span>|<span data-ttu-id="102d3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="102d3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="102d3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="102d3-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="102d3-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="102d3-118">Request headers</span></span>
|<span data-ttu-id="102d3-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="102d3-119">Header</span></span>|<span data-ttu-id="102d3-120">Значение</span><span class="sxs-lookup"><span data-stu-id="102d3-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="102d3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="102d3-121">Authorization</span></span>|<span data-ttu-id="102d3-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="102d3-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="102d3-123">Accept</span><span class="sxs-lookup"><span data-stu-id="102d3-123">Accept</span></span>|<span data-ttu-id="102d3-124">application/json</span><span class="sxs-lookup"><span data-stu-id="102d3-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="102d3-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="102d3-125">Request body</span></span>
<span data-ttu-id="102d3-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="102d3-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="102d3-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="102d3-127">Response</span></span>
<span data-ttu-id="102d3-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [roleAssignment](../resources/intune-rbac-roleassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="102d3-128">If successful, this method returns a `200 OK` response code and a collection of [roleAssignment](../resources/intune-rbac-roleassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="102d3-129">Пример</span><span class="sxs-lookup"><span data-stu-id="102d3-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="102d3-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="102d3-130">Request</span></span>
<span data-ttu-id="102d3-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="102d3-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
```

### <a name="response"></a><span data-ttu-id="102d3-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="102d3-132">Response</span></span>
<span data-ttu-id="102d3-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="102d3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 303

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.roleAssignment",
      "id": "b3234d24-4d24-b323-244d-23b3244d23b3",
      "displayName": "Display Name value",
      "description": "Description value",
      "resourceScopes": [
        "Resource Scopes value"
      ]
    }
  ]
}
```



