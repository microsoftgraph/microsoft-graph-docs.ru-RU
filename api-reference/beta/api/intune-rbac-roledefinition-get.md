---
title: Получение roleDefinition
description: Чтение свойств и связей объекта roleDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1c7e4229fd8cb9ab1206262a833746a5d970344c
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51141570"
---
# <a name="get-roledefinition"></a><span data-ttu-id="721ab-103">Получение roleDefinition</span><span class="sxs-lookup"><span data-stu-id="721ab-103">Get roleDefinition</span></span>

<span data-ttu-id="721ab-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="721ab-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="721ab-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="721ab-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="721ab-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="721ab-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="721ab-107">Чтение свойств и связей объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="721ab-107">Read properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="721ab-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="721ab-108">Prerequisites</span></span>
<span data-ttu-id="721ab-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="721ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="721ab-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="721ab-111">Permission type</span></span>|<span data-ttu-id="721ab-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="721ab-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="721ab-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="721ab-113">Delegated (work or school account)</span></span>|<span data-ttu-id="721ab-114">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="721ab-114">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="721ab-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="721ab-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="721ab-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="721ab-116">Not supported.</span></span>|
|<span data-ttu-id="721ab-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="721ab-117">Application</span></span>|<span data-ttu-id="721ab-118">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="721ab-118">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="721ab-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="721ab-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions/{roleDefinitionId}
GET /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="optional-query-parameters"></a><span data-ttu-id="721ab-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="721ab-120">Optional query parameters</span></span>
<span data-ttu-id="721ab-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="721ab-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="721ab-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="721ab-122">Request headers</span></span>
|<span data-ttu-id="721ab-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="721ab-123">Header</span></span>|<span data-ttu-id="721ab-124">Значение</span><span class="sxs-lookup"><span data-stu-id="721ab-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="721ab-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="721ab-125">Authorization</span></span>|<span data-ttu-id="721ab-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="721ab-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="721ab-127">Accept</span><span class="sxs-lookup"><span data-stu-id="721ab-127">Accept</span></span>|<span data-ttu-id="721ab-128">application/json</span><span class="sxs-lookup"><span data-stu-id="721ab-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="721ab-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="721ab-129">Request body</span></span>
<span data-ttu-id="721ab-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="721ab-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="721ab-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="721ab-131">Response</span></span>
<span data-ttu-id="721ab-132">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [roleDefinition](../resources/intune-rbac-roledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="721ab-132">If successful, this method returns a `200 OK` response code and [roleDefinition](../resources/intune-rbac-roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="721ab-133">Пример</span><span class="sxs-lookup"><span data-stu-id="721ab-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="721ab-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="721ab-134">Request</span></span>
<span data-ttu-id="721ab-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="721ab-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}
```

### <a name="response"></a><span data-ttu-id="721ab-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="721ab-136">Response</span></span>
<span data-ttu-id="721ab-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="721ab-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




