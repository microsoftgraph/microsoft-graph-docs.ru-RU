---
title: Получение roleDefinition
description: Чтение свойств и связей объекта roleDefinition.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 787c10e663f465353ead334b8dc9ffc9ee866a12
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418640"
---
# <a name="get-roledefinition"></a><span data-ttu-id="08edd-103">Получение roleDefinition</span><span class="sxs-lookup"><span data-stu-id="08edd-103">Get roleDefinition</span></span>

> <span data-ttu-id="08edd-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="08edd-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="08edd-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08edd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="08edd-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="08edd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08edd-107">Чтение свойств и связей объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="08edd-107">Read properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="08edd-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="08edd-108">Prerequisites</span></span>
<span data-ttu-id="08edd-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="08edd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="08edd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="08edd-111">Permission type</span></span>|<span data-ttu-id="08edd-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="08edd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="08edd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="08edd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="08edd-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="08edd-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="08edd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="08edd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="08edd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08edd-116">Not supported.</span></span>|
|<span data-ttu-id="08edd-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="08edd-117">Application</span></span>|<span data-ttu-id="08edd-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08edd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="08edd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="08edd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions/{roleDefinitionId}
GET /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="optional-query-parameters"></a><span data-ttu-id="08edd-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="08edd-120">Optional query parameters</span></span>
<span data-ttu-id="08edd-121">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="08edd-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="08edd-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="08edd-122">Request headers</span></span>
|<span data-ttu-id="08edd-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="08edd-123">Header</span></span>|<span data-ttu-id="08edd-124">Значение</span><span class="sxs-lookup"><span data-stu-id="08edd-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="08edd-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="08edd-125">Authorization</span></span>|<span data-ttu-id="08edd-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="08edd-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="08edd-127">Accept</span><span class="sxs-lookup"><span data-stu-id="08edd-127">Accept</span></span>|<span data-ttu-id="08edd-128">application/json</span><span class="sxs-lookup"><span data-stu-id="08edd-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="08edd-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="08edd-129">Request body</span></span>
<span data-ttu-id="08edd-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="08edd-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="08edd-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="08edd-131">Response</span></span>
<span data-ttu-id="08edd-132">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [roleDefinition](../resources/intune-rbac-roledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="08edd-132">If successful, this method returns a `200 OK` response code and [roleDefinition](../resources/intune-rbac-roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08edd-133">Пример</span><span class="sxs-lookup"><span data-stu-id="08edd-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="08edd-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="08edd-134">Request</span></span>
<span data-ttu-id="08edd-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="08edd-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}
```

### <a name="response"></a><span data-ttu-id="08edd-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="08edd-136">Response</span></span>
<span data-ttu-id="08edd-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="08edd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




