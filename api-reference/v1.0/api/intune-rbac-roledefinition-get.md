---
title: Получение roleDefinition
description: Чтение свойств и связей объекта roleDefinition.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 64b9f0cb9c00ac631c45935e547387cc9e9bcd2d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36025951"
---
# <a name="get-roledefinition"></a><span data-ttu-id="a40ce-103">Получение roleDefinition</span><span class="sxs-lookup"><span data-stu-id="a40ce-103">Get roleDefinition</span></span>

> <span data-ttu-id="a40ce-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a40ce-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a40ce-105">Чтение свойств и связей объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="a40ce-105">Read properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a40ce-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a40ce-106">Prerequisites</span></span>
<span data-ttu-id="a40ce-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a40ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a40ce-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a40ce-109">Permission type</span></span>|<span data-ttu-id="a40ce-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a40ce-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a40ce-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a40ce-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a40ce-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="a40ce-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="a40ce-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a40ce-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a40ce-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a40ce-114">Not supported.</span></span>|
|<span data-ttu-id="a40ce-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a40ce-115">Application</span></span>|<span data-ttu-id="a40ce-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a40ce-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a40ce-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a40ce-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions/{roleDefinitionId}
GET /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a40ce-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a40ce-118">Optional query parameters</span></span>
<span data-ttu-id="a40ce-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a40ce-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a40ce-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a40ce-120">Request headers</span></span>
|<span data-ttu-id="a40ce-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a40ce-121">Header</span></span>|<span data-ttu-id="a40ce-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a40ce-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a40ce-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a40ce-123">Authorization</span></span>|<span data-ttu-id="a40ce-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a40ce-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a40ce-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a40ce-125">Accept</span></span>|<span data-ttu-id="a40ce-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a40ce-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a40ce-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a40ce-127">Request body</span></span>
<span data-ttu-id="a40ce-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a40ce-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a40ce-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="a40ce-129">Response</span></span>
<span data-ttu-id="a40ce-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [roleDefinition](../resources/intune-rbac-roledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a40ce-130">If successful, this method returns a `200 OK` response code and [roleDefinition](../resources/intune-rbac-roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a40ce-131">Пример</span><span class="sxs-lookup"><span data-stu-id="a40ce-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="a40ce-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="a40ce-132">Request</span></span>
<span data-ttu-id="a40ce-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a40ce-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions/{roleDefinitionId}
```

### <a name="response"></a><span data-ttu-id="a40ce-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="a40ce-134">Response</span></span>
<span data-ttu-id="a40ce-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a40ce-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



