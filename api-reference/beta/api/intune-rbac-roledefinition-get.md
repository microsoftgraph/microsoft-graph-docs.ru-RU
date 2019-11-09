---
title: Получение roleDefinition
description: Чтение свойств и связей объекта roleDefinition.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: df12c42c88c50992e564f3b90648c04af4c7b519
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/09/2019
ms.locfileid: "38086384"
---
# <a name="get-roledefinition"></a><span data-ttu-id="75429-103">Получение roleDefinition</span><span class="sxs-lookup"><span data-stu-id="75429-103">Get roleDefinition</span></span>

> <span data-ttu-id="75429-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75429-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="75429-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="75429-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75429-106">Чтение свойств и связей объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="75429-106">Read properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="75429-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="75429-107">Prerequisites</span></span>
<span data-ttu-id="75429-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75429-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75429-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="75429-110">Permission type</span></span>|<span data-ttu-id="75429-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="75429-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="75429-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="75429-112">Delegated (work or school account)</span></span>|<span data-ttu-id="75429-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="75429-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="75429-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="75429-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="75429-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75429-115">Not supported.</span></span>|
|<span data-ttu-id="75429-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="75429-116">Application</span></span>|<span data-ttu-id="75429-117">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="75429-117">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="75429-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="75429-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions/{roleDefinitionId}
GET /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="optional-query-parameters"></a><span data-ttu-id="75429-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="75429-119">Optional query parameters</span></span>
<span data-ttu-id="75429-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="75429-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="75429-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="75429-121">Request headers</span></span>
|<span data-ttu-id="75429-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="75429-122">Header</span></span>|<span data-ttu-id="75429-123">Значение</span><span class="sxs-lookup"><span data-stu-id="75429-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="75429-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="75429-124">Authorization</span></span>|<span data-ttu-id="75429-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="75429-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="75429-126">Accept</span><span class="sxs-lookup"><span data-stu-id="75429-126">Accept</span></span>|<span data-ttu-id="75429-127">application/json</span><span class="sxs-lookup"><span data-stu-id="75429-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="75429-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="75429-128">Request body</span></span>
<span data-ttu-id="75429-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="75429-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="75429-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="75429-130">Response</span></span>
<span data-ttu-id="75429-131">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [roleDefinition](../resources/intune-rbac-roledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="75429-131">If successful, this method returns a `200 OK` response code and [roleDefinition](../resources/intune-rbac-roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75429-132">Пример</span><span class="sxs-lookup"><span data-stu-id="75429-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="75429-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="75429-133">Request</span></span>
<span data-ttu-id="75429-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="75429-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}
```

### <a name="response"></a><span data-ttu-id="75429-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="75429-135">Response</span></span>
<span data-ttu-id="75429-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="75429-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






