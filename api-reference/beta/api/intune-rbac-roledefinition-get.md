---
title: Получение roleDefinition
description: Чтение свойств и связей объекта roleDefinition.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e409291bad51a6693823aaf7eb74929f176057c1
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33899426"
---
# <a name="get-roledefinition"></a><span data-ttu-id="00a92-103">Получение roleDefinition</span><span class="sxs-lookup"><span data-stu-id="00a92-103">Get roleDefinition</span></span>

> <span data-ttu-id="00a92-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00a92-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="00a92-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="00a92-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00a92-106">Чтение свойств и связей объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="00a92-106">Read properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="00a92-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="00a92-107">Prerequisites</span></span>
<span data-ttu-id="00a92-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00a92-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00a92-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="00a92-110">Permission type</span></span>|<span data-ttu-id="00a92-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="00a92-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="00a92-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="00a92-112">Delegated (work or school account)</span></span>|<span data-ttu-id="00a92-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="00a92-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="00a92-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="00a92-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="00a92-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00a92-115">Not supported.</span></span>|
|<span data-ttu-id="00a92-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="00a92-116">Application</span></span>|<span data-ttu-id="00a92-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00a92-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="00a92-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="00a92-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions/{roleDefinitionId}
GET /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="optional-query-parameters"></a><span data-ttu-id="00a92-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="00a92-119">Optional query parameters</span></span>
<span data-ttu-id="00a92-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="00a92-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="00a92-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="00a92-121">Request headers</span></span>
|<span data-ttu-id="00a92-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="00a92-122">Header</span></span>|<span data-ttu-id="00a92-123">Значение</span><span class="sxs-lookup"><span data-stu-id="00a92-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="00a92-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="00a92-124">Authorization</span></span>|<span data-ttu-id="00a92-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="00a92-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="00a92-126">Accept</span><span class="sxs-lookup"><span data-stu-id="00a92-126">Accept</span></span>|<span data-ttu-id="00a92-127">application/json</span><span class="sxs-lookup"><span data-stu-id="00a92-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="00a92-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="00a92-128">Request body</span></span>
<span data-ttu-id="00a92-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="00a92-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="00a92-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="00a92-130">Response</span></span>
<span data-ttu-id="00a92-131">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [roleDefinition](../resources/intune-rbac-roledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="00a92-131">If successful, this method returns a `200 OK` response code and [roleDefinition](../resources/intune-rbac-roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00a92-132">Пример</span><span class="sxs-lookup"><span data-stu-id="00a92-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="00a92-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="00a92-133">Request</span></span>
<span data-ttu-id="00a92-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="00a92-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}
```

### <a name="response"></a><span data-ttu-id="00a92-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="00a92-135">Response</span></span>
<span data-ttu-id="00a92-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="00a92-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1369

{
  "value": {
    "@odata.type": "#microsoft.graph.roleDefinition",
    "id": "70fdcd08-cd08-70fd-08cd-fd7008cdfd70",
    "displayName": "Display Name value",
    "description": "Description value",
    "permissions": [
      {
        "@odata.type": "microsoft.graph.rolePermission",
        "actions": [
          "Actions value"
        ],
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
    "rolePermissions": [
      {
        "@odata.type": "microsoft.graph.rolePermission",
        "actions": [
          "Actions value"
        ],
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
    "isBuiltInRoleDefinition": true,
    "isBuiltIn": true,
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ]
  }
}
```




