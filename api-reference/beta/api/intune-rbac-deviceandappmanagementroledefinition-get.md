---
title: Получение deviceAndAppManagementRoleDefinition
description: Считывание свойств и связей объекта deviceAndAppManagementRoleDefinition.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6f3326522873af571b84c27d8c6011fa2de5e254
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39940695"
---
# <a name="get-deviceandappmanagementroledefinition"></a><span data-ttu-id="3196b-103">Получение deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="3196b-103">Get deviceAndAppManagementRoleDefinition</span></span>

> <span data-ttu-id="3196b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3196b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3196b-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3196b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3196b-106">Считывание свойств и связей объекта [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="3196b-106">Read properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3196b-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="3196b-107">Prerequisites</span></span>
<span data-ttu-id="3196b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3196b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3196b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3196b-110">Permission type</span></span>|<span data-ttu-id="3196b-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3196b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3196b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3196b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3196b-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="3196b-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="3196b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3196b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3196b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3196b-115">Not supported.</span></span>|
|<span data-ttu-id="3196b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3196b-116">Application</span></span>|<span data-ttu-id="3196b-117">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="3196b-117">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3196b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3196b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions/{roleDefinitionId}
GET /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3196b-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3196b-119">Optional query parameters</span></span>
<span data-ttu-id="3196b-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3196b-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3196b-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3196b-121">Request headers</span></span>
|<span data-ttu-id="3196b-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3196b-122">Header</span></span>|<span data-ttu-id="3196b-123">Значение</span><span class="sxs-lookup"><span data-stu-id="3196b-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3196b-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3196b-124">Authorization</span></span>|<span data-ttu-id="3196b-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3196b-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3196b-126">Accept</span><span class="sxs-lookup"><span data-stu-id="3196b-126">Accept</span></span>|<span data-ttu-id="3196b-127">application/json</span><span class="sxs-lookup"><span data-stu-id="3196b-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3196b-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3196b-128">Request body</span></span>
<span data-ttu-id="3196b-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3196b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3196b-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="3196b-130">Response</span></span>
<span data-ttu-id="3196b-131">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3196b-131">If successful, this method returns a `200 OK` response code and [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3196b-132">Пример</span><span class="sxs-lookup"><span data-stu-id="3196b-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="3196b-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="3196b-133">Request</span></span>
<span data-ttu-id="3196b-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3196b-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}
```

### <a name="response"></a><span data-ttu-id="3196b-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="3196b-135">Response</span></span>
<span data-ttu-id="3196b-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3196b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1391

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleDefinition",
    "id": "bca1dfb5-dfb5-bca1-b5df-a1bcb5dfa1bc",
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





