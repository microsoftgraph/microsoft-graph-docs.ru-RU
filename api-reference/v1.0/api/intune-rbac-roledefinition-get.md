---
title: Получение roleDefinition
description: Чтение свойств и связей объекта roleDefinition.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ae3eb37f3a3a3a0d835d405b89d5ab5102c3e43e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947115"
---
# <a name="get-roledefinition"></a><span data-ttu-id="8d0ca-103">Получение roleDefinition</span><span class="sxs-lookup"><span data-stu-id="8d0ca-103">Get roleDefinition</span></span>

> <span data-ttu-id="8d0ca-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8d0ca-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8d0ca-105">Чтение свойств и связей объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="8d0ca-105">Read properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8d0ca-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8d0ca-106">Prerequisites</span></span>
<span data-ttu-id="8d0ca-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d0ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d0ca-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8d0ca-109">Permission type</span></span>|<span data-ttu-id="8d0ca-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8d0ca-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8d0ca-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8d0ca-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8d0ca-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="8d0ca-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="8d0ca-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8d0ca-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d0ca-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d0ca-114">Not supported.</span></span>|
|<span data-ttu-id="8d0ca-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8d0ca-115">Application</span></span>|<span data-ttu-id="8d0ca-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d0ca-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d0ca-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8d0ca-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions/{roleDefinitionId}
GET /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8d0ca-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8d0ca-118">Optional query parameters</span></span>
<span data-ttu-id="8d0ca-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8d0ca-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="8d0ca-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8d0ca-120">Request headers</span></span>
|<span data-ttu-id="8d0ca-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8d0ca-121">Header</span></span>|<span data-ttu-id="8d0ca-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8d0ca-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8d0ca-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d0ca-123">Authorization</span></span>|<span data-ttu-id="8d0ca-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="8d0ca-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8d0ca-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8d0ca-125">Accept</span></span>|<span data-ttu-id="8d0ca-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8d0ca-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d0ca-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8d0ca-127">Request body</span></span>
<span data-ttu-id="8d0ca-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8d0ca-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8d0ca-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d0ca-129">Response</span></span>
<span data-ttu-id="8d0ca-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [roleDefinition](../resources/intune-rbac-roledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8d0ca-130">If successful, this method returns a `200 OK` response code and [roleDefinition](../resources/intune-rbac-roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d0ca-131">Пример</span><span class="sxs-lookup"><span data-stu-id="8d0ca-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="8d0ca-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="8d0ca-132">Request</span></span>
<span data-ttu-id="8d0ca-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8d0ca-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions/{roleDefinitionId}
```

### <a name="response"></a><span data-ttu-id="8d0ca-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="8d0ca-134">Response</span></span>
<span data-ttu-id="8d0ca-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="8d0ca-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 690

{
  "value": {
    "@odata.type": "#microsoft.graph.roleDefinition",
    "id": "70fdcd08-cd08-70fd-08cd-fd7008cdfd70",
    "displayName": "Display Name value",
    "description": "Description value",
    "rolePermissions": [
      {
        "@odata.type": "microsoft.graph.rolePermission",
        "resourceActions": [
          {
            "@odata.type": "microsoft.graph.resourceAction",
            "allowedResourceActions": [
              "Allowed Resource Actions value"
            ],
            "notAllowedResourceActions": [
              "Not Allowed Resource Actions value"
            ]
          }
        ]
      }
    ],
    "isBuiltIn": true
  }
}
```



